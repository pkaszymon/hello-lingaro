<script>
import HelloWorld from "@/components/HelloWorld.vue"
import { defineComponent } from "vue";

export default defineComponent({
  components: {
    HelloWorld
  }
})

</script>

<template>
  <main>
    
    <HelloWorld title="Hello Lingaro!" msg="I deployed this Vue.js app using Azure Static Web App resource." />
  </main>
</template>

<style>
.message {
  text-align: center;
  /* width: 100%; */
  margin: 3rem;
}
</style>