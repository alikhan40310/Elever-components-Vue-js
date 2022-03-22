<template>
  <main class="container-fluid">
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

<script>
// import experience
import Experience from "./Experience.vue";
// import bars
import Bars from "./Bars.vue";
export default {
  name: "App",
  components: {
    Experience,
    Bars,
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

<style>
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
