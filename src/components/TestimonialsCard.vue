<template>
  <div
    v-for="(item, index) in testimonials"
    :key="index"
    class="testimonial"
    :class="[item.tag]"
  >
    <div class="testimonial_user">
      <img :src="item.img" alt="" />
      <div class="name">
        <h3>{{ item.name }}</h3>
        <span class="status">{{ item.profession }}</span>
      </div>
    </div>
    <div class="testimonia-container">
      <h2>
        {{ item.title }}
      </h2>
      <p>
        {{ item.description }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    testimonials: { default: [] },
  },
};
</script>

<style></style>
