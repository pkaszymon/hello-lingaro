<script>
import HelloWorld from '@/components/HelloWorld.vue'


export default {
  data() {
    return {
      message: ""
    };
  }
}

</script>

<template>
  <main>
    <HelloWorld title="Hello Lingaro!" msg="I deployed this Vue.js app using Azure Static Web App resource." />
  </main>
  {{  message }}
</template>
