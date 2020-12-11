<template>
  <div id="app">
    <my-header :navItems="navItems"></my-header>
    <my-body :aTitle="myTitle"></my-body>
    <my-footer :aCopyright="myCopyright"></my-footer>
  </div>
</template>

<script>
import MyHeader from "./components/my-header";
import MyBody from "./components/my-body";
import MyFooter from "./components/my-footer";

export default {
  name: "App",
  components: {
    MyHeader,
    MyBody,
    MyFooter,
  },
  data() {
    return {
      myTitle: "My Vue App",
      myCopyright: "@Juan",
      navItems: [
        {
          name: "Home",
          href: "/index.html",
        },
        {
          name: "About",
          href: "/about.html",
        },
        {
          name: "Contact",
          href: "/contact.html",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
