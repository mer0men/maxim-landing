<template>
  <div id="app">
    <navbar></navbar>
    <offer></offer>
    <cases></cases>
    <speakers></speakers>
    <contacts></contacts>
  </div>
</template>

<script>
import navbar from "@/components/Navbar";
import cases from "@/components/Cases";
import contacts from "@/components/Contacts";
import offer from "@/components/Offer";
import speakers from "@/components/Speakers";

export default {
  name: "app",
  components: {
    navbar,
    cases,
    contacts,
    offer,
    speakers
  }
};
</script>

<style lang="scss">
@font-face {
  font-family: "permian";
  src: url(./assets/permiansanstypeface.ttf);
}

body,
html {
  margin: 0;
  padding: 0;
}

#app {
  font-family: "permian", sans-serif;
  background: white;
  position: relative;
}

.btn {
  width: 30%;
  height: 65px;
  background: white;
  font-size: 24px;
  line-height: 38px;
  color: #e52600;
  border: 1px solid #e52600;
  box-sizing: border-box;
  border-radius: 60px;
  text-transform: lowercase;
  margin: 8px;
  transition: 0.4s;
  cursor: pointer;

  &:focus {
    outline: 0;
  }

  &:hover {
    background: #e52600;
    color: white;
  }
}
</style>
