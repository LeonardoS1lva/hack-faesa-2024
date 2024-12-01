<template>
  <div class="card" :style="{ width: width }">
    <div class="container">
      <h4>
        <b>{{ title }}</b>
      </h4>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
    width: {
      type: String,
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.card {
  /* background-color: #d9d9d9; */
  background: linear-gradient(285deg, rgba(16, 69, 99, 0.90) 3.74%, rgba(5, 45, 67, 0.89) 52.63%, #032030 101.8%);
color: #fff;
  border-radius: 5px;
  padding: 2rem;
  margin-top: 2rem;
  border-radius: 1.5rem;
}
</style>
