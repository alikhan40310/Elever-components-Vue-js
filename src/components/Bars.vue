<template>
  <div class="container">
    <div class="content">
      <h4>{{ subTitle }}</h4>
      <h2>{{ title }}</h2>
      <p>{{ detail }}</p>
    </div>
    <div class="viewBar">
      <div
        class="d-flex mb-3"
        v-for="(progressBar, index) in progressBars"
        :key="index"
      >
        <div class="item cus-bg p-3">
          <div class="d-flex">
            <p class="pr-2">{{ progressBar.progress }}%</p>
            <p class="">{{ progressBar.install }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "",
  data() {
    return {
      title: "cyberdyne Systems",
      subTitle: "Organization",
      detail: " 1223 Students ",
      message: "",
      show: true,
      progressBars: [
        {
          progress: 0.0,
          install: "Android",
        },
        {
          progress: 0.1,
          install: "iOS",
        },
        {
          progress: 0.3,
          install: "Web",
        },
      ],
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
.content h4 {
  font-size: 1.2rem;
}
.content h2 {
  text-transform: capitalize;
}
.item {
  width: 100%;
  /* height: 6rem; */
  /* padding: 1rem; */
}
.item p {
  font-size: 1.4rem;
  font-weight: 500;
}
.pr-2 {
  margin-right: 1rem;
  /* width: 100%; */
}
.cus-bg {
  background-color: #b9dbd9;
}
</style>
