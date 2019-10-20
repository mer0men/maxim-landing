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
  margin: 24px 56px;
  background: white;
  position: relative;
}

.btn {
  width: 20%;
  background: white;
  font-size: 30px;
  line-height: 38px;
  color: #e52600;
  border: 1px solid #e52600;
  box-sizing: border-box;
  border-radius: 60px;

  &:focus {
    outline: 0;
  }
}
</style>
