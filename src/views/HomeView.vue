<script>
import HelloWorld from '@/components/HelloWorld.vue'


export default {
  data() {
    return {
      message: ""
    };
  },
  async mounted() {
    const resp = await fetch("/api/message");
    console.log(resp);
    const { text } = await resp.json();
    this.message = text; 
  }
}
</script>

<template>
  <main>
    <HelloWorld title="Hello Lingaro!" msg="I deployed this Vue.js app using Azure Static Web App resource." />
  </main>
  {{  message }}
</template>
