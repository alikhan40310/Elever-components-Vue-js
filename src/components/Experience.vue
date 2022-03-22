<template>
  <div class="container">
    <div class="context mt-5">
      <h5>{{ title }}</h5>
      <div class="content">
        <div class="row">
          <div
            class="col-md-3"
            v-for="(experience, index) in experiences"
            :key="index"
          >
            <div class="main rounded-full col-md-12 mt-5">
              <div class="inner" :class="experience.color">
                <h4>{{ experience.mainTitle }}</h4>
                <h2>{{ experience.value }}</h2>
              </div>
              <div class="text p-3">
                <div class="d-flex flex-column">
                  <h4 class="fs-6 fw-bold">{{ experience.title }}</h4>
                  <span>{{ experience.group }}</span>
                  <span>{{ experience.student }}</span>
                </div>
              </div>
            </div>
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
      title: "Experience",
      experiences: [
        {
          mainTitle: "experience",
          value: "E4",
          title: "E4 Cyberdyne Systems Experience",
          detail: "6 groups, 32 students",
          group: "6 groups",
          student: "32 students",
          color: "bg-danger",
        },
        {
          mainTitle: "experience",
          value: "E4",
          title: "E4 Cyberdyne Systems Experience",
          detail: "6 groups, 32 students",
          group: "6 groups",
          student: "32 students",
          color: "bg-info",

        },
        {
          mainTitle: "experience",
          value: "E4",
          title: "E4 Cyberdyne Systems Experience",
          detail: "6 groups, 32 students",
          group: "6 groups",
          student: "32 students",
          color: "bg-warning",
        },
        {
          mainTitle: "experience",
          value: "E4",
          title: "E4 Cyberdyne Systems Experience",
          detail: "6 groups, 32 students",
          group: "6 groups",
          student: "32 students",
          color: "bg-success",
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
h5 {
  font-size: 1.2rem;
  color: #459a9c;
}

.main {
  border-radius: 0.5rem;
  background-color: rgb(243, 243, 243);
  width: 100%;
  /* padding: 1rem 0; */
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1);
}
.main .inner {
  background-color: #ce5748;
  padding: 1rem;
  color: white;
  border-top-left-radius: 0.5rem;
  border-top-right-radius: 0.5rem;
  text-align: center;
}
</style>
