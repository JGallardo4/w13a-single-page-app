<template>
  <main>
    <h1>{{ aTitle }}</h1>
  </main>
</template>

<script>
export default {
  name: "my-body",
  props: {
    aTitle: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
</style>