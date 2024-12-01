<template>
  <div class="notFound">
    <h1>404</h1>
    <p>Page not found</p>
  </div>
</template>

<script>
export default {
  name: "NotFound",
};
</script>

<style scoped>
.notFound {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-size: 2rem;
  color: #333;
}
</style>
