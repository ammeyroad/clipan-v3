<template>
  <section class="text-gray-600 body-font relative">
    <div class="container px-5 py-24 mx-auto flex sm:flex-nowrap flex-wrap">

      <div
        class="
          lg:w-1/3
          md:w-1/2
          bg-white
          flex flex-col
          md:ml-auto
          w-full
          md:py-8
          mt-8
          md:mt-0
          p-5
        "
      >
        <h2 class="text-gray-900 text-2xl mb-1 font-bold title-font">
          Send us a Message now
        </h2>
        <p class="leading-relaxed mb-5 text-gray-600 text-md">
          You are only a few steps away from obtaining the information you
          require. However, if you send the message now, our team will contact
          you right away
        </p>
        <form name="contact" method="POST" netlify>
          <p><input type="hidden" name="form-name" value="contact" /></p>
          <div class="relative mb-4">
            <label for="name" class="leading-7 text-sm text-gray-600"
              >Name</label
            >
            <input
              type="text"
              id="name"
              name="name"
              class="
                w-full
                bg-white
                rounded
                border border-gray-300
                focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200
                text-base
                outline-none
                text-gray-700
                py-1
                px-3
                leading-8
                transition-colors
                duration-200
                ease-in-out
              "
              v-model="form.name"
            />
          </div>
          <div class="relative mb-4">
            <label for="email" class="leading-7 text-sm text-gray-600"
              >Email</label
            >
            <input
              type="email"
              id="email"
              name="email"
              class="
                w-full
                bg-white
                rounded
                border border-gray-300
                focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200
                text-base
                outline-none
                text-gray-700
                py-1
                px-3
                leading-8
                transition-colors
                duration-200
                ease-in-out
              "
              v-model="form.email"
            />
          </div>
          <div class="relative mb-4">
            <label for="message" class="leading-7 text-sm text-gray-600"
              >Message</label
            >
            <textarea
              id="message"
              name="message"
              class="
                w-full
                bg-white
                rounded
                border border-gray-300
                focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200
                h-32
                text-base
                outline-none
                text-gray-700
                py-1
                px-3
                resize-none
                leading-6
                transition-colors
                duration-200
                ease-in-out
              "
              v-model="form.message"
            ></textarea>
          </div>
          <button
            class="
              text-white
              bg-indigo-500
              border-0
              py-2
              px-6
              focus:outline-none
              hover:bg-indigo-600
              rounded
              text-lg
            "
            type="submit"
            @click.prevent="formSubmit"
          >
            Send
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: '',
        email: '',
        message: '',
      },
    };
  },
  methods: {
    encode(data) {
      return Object.keys(data)
        .map(
          (key) => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`
        )
        .join('&');
    },
    formSubmit() {
      fetch('/', {
        method: 'POST',
        headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
        body: this.encode({ 'form-name': 'contact', ...this.form }),
      })
        .then(() => console.log('You have sucessfully submitted the form'))
        .catch((error) => alert(error));
    },
  },
};
</script>
