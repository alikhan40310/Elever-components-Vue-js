<script>
// import bars
import Bars from "./components/Bars.vue";
// import experience
import Experience from "./components/Experience.vue";
// import organization
import Organization from "./components/Organization.vue";
// import organizationexperience
import OrganizationExperience from "./components/OrganizationExperience.vue";
// import bootstrap
import "bootstrap/dist/css/bootstrap.min.css";

export default {
  name: "App",
  components: {
    Organization,
    Bars,
    Experience,
    OrganizationExperience,
  },
  data() {
    return {
      title: "Hello Vue!",
      message: "This is a message from the App component",
      show: true,
    };
  },
  methods: {
    MyFunction() {

    },
  },
};
</script>

<template >
  <Organization />
</template>

<style>
@import "./assets/base.css";


</style>
