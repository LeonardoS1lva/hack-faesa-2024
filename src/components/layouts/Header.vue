<template>
  <div class="cabecario">
    <slot name="title"></slot>
    <NavLinks :navLi1="nav1" :navLi2="nav2" :navLi3="nav3" :navLi4="nav4" :link1="link1" :link2="link2" :link3="link3" :link4="link4" /> 
  </div>
</template>

<script>
import NavLinks from "@/components/layouts/NavLinks.vue";

export default {
  components: {
    NavLinks,
  },
  props: {
    title: {
      type: [String, Object],
      required: false,
    },
    nav1: {
      type: String,
      required: true,
    },
    nav2: {
      type: String,
      required: true,
    },
    nav3: {
      type: String,
      required: true,
    },
    nav4: {
      type: String,
      required: true,
    },
    link1: {
      type: String,
      required: false,
    },
    link2: {
      type: String,
      required: false,
    },
    link3: {
      type: String,
      required: false,
    },
    link4: {
      type: String,
      required: false,
    },
  },
};
</script>

<style scoped>
.cabecario {
  /* background-color: #333; */
  background: linear-gradient(285deg, rgba(16, 69, 99, 0.90) 3.74%, rgba(5, 45, 67, 0.89) 52.63%, #032030 101.8%);

  color: #fff;
  height: 8vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
}
</style>
