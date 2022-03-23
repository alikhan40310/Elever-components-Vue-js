<template>
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
</template>

<script>
export default {
  name: "OrganizationExperience",
  props: {
    experience: {
      type: Object,
      required: true,
    },
    index: {
      type: Number,
      required: true,
    },
  },
  data() {
    return {
      title: "Experience",
    };
  },
  methods: {
    MyFunction() {},
  },
};
</script>

<style></style>
