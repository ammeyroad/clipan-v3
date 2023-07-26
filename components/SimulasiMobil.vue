<template>
  <div class="container mx-auto p-4">
    <h1 class="text-2xl font-bold mb-4">Car Loan Calculator</h1>
    <form @submit.prevent="calculateInstallments">
      <div class="mb-2">
        <label for="hargaotr" class="block font-bold">Harga OTR:</label>
        <input
          type="number"
          id="hargaotr"
          class="w-full p-2 border rounded"
          v-model.number="hargaOtr"
          required
        >
      </div>
      <div class="mb-2">
        <label for="nominalDP" class="block font-bold">Nominal Uang Muka:</label>
        <input
          type="number"
          id="nominalDP"
          class="w-full p-2 border rounded"
          v-model.number="nominalDp"
          required
        >
      </div>
      <div class="mb-2">
        <label for="persenDP" class="block font-bold">Persen Uang Muka:</label>
        <input
          type="number"
          id="persenDP"
          class="w-full p-2 border rounded"
          v-model.number="persenDp"
          required
        >
      </div>
      <button type="submit" class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">
        {{ calculated ? "Recalculate" : "Calculate" }}
      </button>
    </form>
    <div v-if="showInstallments">
      <h2 class="text-lg font-bold mb-2">Installment Options:</h2>
      <div v-for="installment in installments" :key="installment.term" class="mb-2">
        <input
          type="radio"
          :id="`term-${installment.term}`"
          class="mr-2"
          :value="installment.installment"
          v-model="selectedInstallment"
        >
        <label :for="`term-${installment.term}`">{{ installment.term }} Bulan: {{ installment.installment }}</label>
        <span class="ml-4">Total Payment: {{ (nominalDp + installment.installment).toFixed(2) }}</span>
      </div>
    </div>
  </div>
</template>

<script setup>

const hargaOtr = ref(0);
const nominalDp = ref(0);
const persenDp = ref(0);
const calculated = ref(false);
const selectedInstallment = ref(null);

const showInstallments = computed(() => calculated.value && installments.value.length > 0);

const calculateDpNominal = () => {
  nominalDp.value = hargaOtr.value * (persenDp.value / 100);
};

const calculateInstallments = () => {
  calculateDpNominal();
  const terms = [12, 24, 36];
  const installmentOptions = terms.map((term) => {
    const installment = Math.ceil((hargaOtr.value - nominalDp.value) / term / 1000) * 1000;
    return { term, installment };
  });
  installments.value = installmentOptions;
  calculated.value = true;
};

const installments = ref([]);
</script>
