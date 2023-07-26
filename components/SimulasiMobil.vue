<template>
  <div class="container mx-auto p-4">
    <h1 class="text-2xl font-bold mb-4">Car Loan Calculator</h1>
    <form @submit.prevent="calculateLoan">
      <div class="mb-2">
        <label for="otr" class="block font-bold">Harga OTR:</label>
        <input
          type="number"
          id="otr"
          class="w-full p-2 border rounded"
          v-model.number="hargaOtr"
          required
        >
      </div>
      <div class="mb-2">
        <label for="dpPercentage" class="block font-bold">Uang Muka (%):</label>
         <input
          type="number"
          id="dpPercentage"
          class="w-full p-2 border rounded"
          v-model.number="dpPercentage"
          @change="calculateDpNominal"
          required
        >

      </div>
      <div class="mb-2">
        <label for="dpNominal" class="block font-bold">Nominal Uang Muka:</label>
        <input
          type="number"
          id="dpNominal"
          class="w-full p-2 border rounded"
          v-model.number="dpNominal"
          @input="calculateDpPercentage"
          required
        >
      </div>
      <button type="submit" class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">Calculate</button>
    </form>
    <div v-if="installments.length > 0">
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
      </div>
    </div>
  </div>
</template>

<script setup>
const hargaOtr = ref(0);
const dpPercentage = ref(20);
const dpNominal = ref(0);
const selectedInstallment = ref(null);
const installments = ref([]);

const calculateDpNominal = () => {
  dpNominal.value = hargaOtr.value * (dpPercentage.value / 100);
};

const calculateDpPercentage = () => {
  dpPercentage.value = (dpNominal.value / hargaOtr.value) * 100;
};

const calculateLoan = () => {
  calculateDpNominal();
  const terms = [12, 24, 36];
  const installmentOptions = terms.map((term) => {
    const installment = Math.ceil((hargaOtr.value - dpNominal.value) / term / 1000) * 1000;
    return { term, installment };
  });
  installments.value = installmentOptions;
};

watch([hargaOtr, dpNominal, dpPercentage], () => calculateLoan());
</script>
