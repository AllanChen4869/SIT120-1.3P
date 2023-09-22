<template>
    <div>
      <h1>Contact Me</h1>
      <form @submit.prevent="submitForm">
        <input v-model="name" placeholder="Your Name" />
        <input v-model="email" type="email" placeholder="Your Email" />
        <textarea v-model="message" placeholder="Your Message"></textarea>
        <button type="submit">Send</button>
      </form>
    </div>
  </template>
  <script>
export default {
  data() {
    return {
      name: '',
      email: '',
      message: ''
    };
  },
  methods: {
    submitForm() {
      // Handle form submission, like sending an email or saving to database
      console.log(this.name, this.email, this.message);
    }
  }
};
</script>

<style>
form {
  max-width: 500px;
  margin-top: 20px;
}

input, textarea, button {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #e0e0e0;
  border-radius: 4px;
  font-size: 16px;
}

button {
  background-color: #007BFF;
  color: #fff;
  cursor: pointer;
  border: none;
}

button:hover {
  background-color: #0056b3;
}

</style>  