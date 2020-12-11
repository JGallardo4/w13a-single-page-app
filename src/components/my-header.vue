<template>
  <header>
    <nav>
      <a v-for="item in navItems" :key="item.name" :href="item.href">
        {{ item.name }}
      </a>
    </nav>
  </header>
</template>

<script>
export default {
  name: "my-header",
  props: {
    navItems: {
      type: Array,
      required: true,
      default: () => [{ name: "No items provided", href: "#" }],
    },
  },
};
</script>

<style lang="sass" scoped>
</style>>