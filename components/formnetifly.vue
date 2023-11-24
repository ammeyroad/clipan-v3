<template>
 <form name="contact" method="POST" netlify>
                        <p><input type="hidden" name="form-name" value="contact"></p>
                        <div class="relative mb-4">
                            <label for="name" class="leading-7 text-sm text-gray-600">Name</label>
                            <input type="text" id="name" name="name"
                                class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
                                v-model="form.name">
                        </div>
                        <div class="relative mb-4">
                            <label for="email" class="leading-7 text-sm text-gray-600">Email</label>
                            <input type="email" id="email" name="email"
                                class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
                                v-model="form.email">
                        </div>
                        <div class="relative mb-4">
                            <label for="message" class="leading-7 text-sm text-gray-600">Message</label>
                            <textarea id="message" name="message"
                                class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out"
                                v-model="form.message"></textarea>                        </div>
                        <button
                            class="text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg"
                            type="submit" @click.prevent="formSubmit">Send</button>
                    </form>
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
                        key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`
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
                    .catch(error => alert(error));
            },
        },
    };
    </script>
