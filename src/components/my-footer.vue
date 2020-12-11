<template>
  <footer>
    <h1>{{ aCopyright }}</h1>
  </footer>
</template>

<script>
export default {
  name: "my-footer",
  props: {
    aCopyright: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
</style>