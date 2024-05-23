<script>
import HelloWorld from "@/components/HelloWorld.vue"


export default {
  components: {
    HelloWorld
  },
  data() {
    return {
      message: "default message"
    };
  },
  async mounted() {
    const resp = await fetch("/api/message");
    console.log(resp);
    const parsed = await resp.json();
    console.log(parsed); 
    this.message = parsed.message;
  }
}
</script>

<template>
  <main>
    <HelloWorld title="Hello Lingaro!" msg="I deployed this Vue.js app using Azure Static Web App resource." />
  </main>
  <div class="message">
    {{  message }}
  </div>
</template>

<style>
.message {
  text-align: center;
  /* width: 100%; */
  margin: 3rem;
}
</style>