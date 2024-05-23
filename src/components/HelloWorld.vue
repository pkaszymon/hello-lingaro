<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  msg: {
    type: String,
    required: true,
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ title }}</h1>
    <h3>
      {{ msg}}
    </h3>
  </div>
</template>

<style scoped>
.greetings{
  text-align: center;
  margin: auto;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

</style>
