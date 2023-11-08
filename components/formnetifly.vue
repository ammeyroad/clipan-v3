<template>
  <div>
    <form
      name="contact"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
      @submit="handleSubmit"
    >
      <div hidden>
        <label>
          Don’t fill this out: <input name="bot-field" />
        </label>
      </div>
      <div>
        <label>Name:
          <input 
            type="text" 
            name="name"
            v-model="formData.name"
            required
          />
        </label>
      </div>
      <div>
        <label>Email:
          <input 
            type="email" 
            name="email"
            v-model="formData.email"
            required
          />
        </label>
      </div>
      <div>
        <label>Message:
          <textarea 
            name="message"
            v-model="formData.message"
            required
          />
        </label>
      </div>
      <div>
        <label class="subtext" for="checkbox">
          <input type="checkbox" v-model="checked" />
          I certify that this message is not full of odeous lies
        </label>
      </div>
      <div>
        <button 
        class="p-4 bg-blue-400"
          type="submit" 
          :disabled="!checked"
        >
          Send
        </button>
      </div>
    </form>
    <div 
      class="alert"
      :class="formAlert.class"
      v-if="formAlert.show"
    >
      {{ formAlert.msg }}
    </div>
  </div>
</template>

<script>
function encode (data) {
  return Object.keys(data)
    .map(key => encodeURIComponent(key) + '=' + encodeURIComponent(data[key]))
    .join('&')
}
export default {
  data () {
    return {
      formData: {
        name: '',
        email: '',
        message: ''
      },
      checked: false,
      formAlert: {
        show: false,
        msg: '',
        class: ''
      }
    }
  },
  methods: {
    handleSubmit (e) {
      fetch('/', {
        method: 'POST',
        headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
        body: encode({ 'form-name': 'contact', ...this.formData })
      })
        .then(res => {
          if (res.status === 200) {
            this.formData = {
              name: '',
              email: '',
              message: ''
            }
            this.formAlert = {
              show: true,
              msg: 'Thank you for your message.  We will reply to you shortly.',
              class: 'success'
            }
          } else {
            this.formAlert = {
              show: true,
              msg: `There was an error: ${res.status} ${res.statusText}. Try again or email us directly.`,
              class: 'error'
            }
          }
          this.checked = false
        })
        .catch(error => {
          this.formAlert = {
            show: true,
            msg: `${error.message}. Try again or email us directly.`,
            class: 'error'
          }
        })

      e.preventDefault()
    }
  }
}
</script>

<style scoped>
form {
  margin: 1rem;
}
.alert {
  margin: 1rem;
  padding: 1rem;
  color: white;
}
.success {
  background-color: green;
}
.error {
  background-color: red;
}
</style>