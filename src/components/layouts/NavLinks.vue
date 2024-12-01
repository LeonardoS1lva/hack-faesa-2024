<template>
  <nav>
    <ul>
      <a :href="link1">
        <li>{{ navLi1 }}</li>
      </a>
      <a :href="link2">
        <li>{{ navLi2 }}</li>
      </a>
      <a :href="link3">
        <li>{{ navLi3 }}</li>
      </a>
      <a :href="link4">
        <li>{{ navLi4 }}</li>
      </a>
    </ul>
  </nav>
</template>

<script>
export default {
  props: {
    navLi1: {
      type: String,
      required: false,
    },
    navLi2: {
      type: String,
      required: false,
    },
    navLi3: {
      type: String,
      required: false,
    },
    navLi4: {
      type: String,
      required: false,
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

<style>
nav {
  /* background-color: #333; */
  /* color: white; */
  height: 8vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
  font-weight: bold;
}
ul {
  display: flex;
  list-style: none;
}
li {
  margin-right: 1rem;
}

a {
  color: white;
  text-decoration: none;
  cursor: pointer;
}
</style>
