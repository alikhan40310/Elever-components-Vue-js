<script>
// import bars
import Bars from "./components/Bars.vue";
// import experience
import Experience from "./components/Experience.vue";
// import bootstrap
import "bootstrap/dist/css/bootstrap.min.css";

export default {
  name: "App",
  components: {
    Bars,
    Experience,
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
      // this.show = !this.show;
    },
  },
};
</script>

<template >
  <main class="container">
    <div class="itemsCenter">
      <div class="row">
        <div class="col-md-4">
          <Bars></Bars>
        </div>
        <div class="col-md-8">
          <Experience></Experience>
        </div>
      </div>
    </div>
  </main>
</template>

<style>
@import "./assets/base.css";

.itemsCenter {
  position: relative;
  width: 100%;
  background: #fafafa;
  padding: 1rem;
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1);
  border-radius: 0.5rem;
}
main {
  height: 100vh;
   margin-top: 10rem; 
}
</style>
