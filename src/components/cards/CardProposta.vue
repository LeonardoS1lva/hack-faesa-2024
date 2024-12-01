<template>
  <div class="card">
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
.card {
  /* background-color: #d9d9d9; */
  background: linear-gradient(285deg, rgba(16, 69, 99, 0.90) 3.74%, rgba(5, 45, 67, 0.89) 52.63%, #032030 101.8%);
  color: #fff;
  border-radius: 5px;
  /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); */
  width: 80%;
  padding: 1rem;
  margin: 0 auto;
  margin-top: 2rem;
  border-radius: 1.5rem;
  padding-bottom: 5rem;
}
</style>
