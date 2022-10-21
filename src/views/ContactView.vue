<template>
    <div class="contact">
      <h6> Silahkan untuk menghubungi saya</h6>
    <h1>{{ title }}</h1>
    <form @submit.prevent="submit">
      <BaseInput 
      v-model="input.name" 
      name="name" 
      label="Name" 
      type="text" />
      <BaseInput
        v-model="input.email"
        name="email"
        label="Email"
        type="email" />

        <BaseInput v-model="input.chat" name="chat" label="chat" type="text" />
      <button type="submit">Submit</button>
    </form>
  </div>
    
  </template>

  <script>
import BaseInput from "@/components/BaseInput.vue";

export default {
  name: "contact",
  components: {
    BaseInput,
  },
  data: () => ({
    title: "Contact",
    // input
    input: {
      name: "",
      email: "",
      class: "",
    },
    //UI
    dropdown: {
      class: ["A", "B", "C",],
    },
  }),
  methods: {
    submit() {
      console.log(this.input);
    }
  },
};
</script>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}
</style>
  