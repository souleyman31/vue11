<template>
  <footer>
    <p>Copyright &copy; 2021</p>
    <!-- <a href="/#about"> About</a> -->
    <router-link to="/about"> About</router-link>
  </footer>
</template>
<script>
export default {
  name: "Footer"
};
</script>
<style scoped>
a {
  color: #656565;
}
footer {
  margin-top: 20px;
  text-align: center;
}
</style>
