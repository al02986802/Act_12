<template>
  <div class="card h-100">
    <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
    <div class="card-body">
      <p class="card-text">{{ value }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ChuckCard",
  props: {
    iconUrl: {
      type: String,
      required: true,
    },
    value: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}
</style>
