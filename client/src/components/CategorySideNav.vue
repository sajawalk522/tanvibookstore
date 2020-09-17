<template>
  <nav id="category-nav">
    <h5>Categories:</h5>
    <ul id="categoryButtons">
      <li class="active">
        <router-link to="#">Romance</router-link>
      </li>
      <li>
        <router-link to="#">Fiction</router-link>
      </li>
      <li>
        <router-link to="#">Business and Finance</router-link>
      </li>
      <li>
        <router-link to="#">Cookbooks</router-link>
      </li>
      <li>
        <router-link to="#">Mystery</router-link>
      </li>
      <li>
        <router-link to="#">Comic Book</router-link>
      </li>
      <li>
        <router-link to="#">Sci-Fi</router-link>
      </li>
      <li>
        <router-link to="#">Action and Adventure</router-link>
      </li>
      <li>
        <router-link to="#" href="#">Poetry</router-link>
      </li>
      <li>
        <router-link to="#" href="#">Historical</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "CategorySideNav",
  data: function() {
    return {};
  }
};
</script>
<style scoped>
#category-nav {
  width: 25%;
  text-align: left;
  border-right: 2px solid #000;
}
#category-nav h5 {
  background-color: #fbe5d6;
  color: #e07517;
  padding: 10px;
  font-size: 20px;
}
#categoryButtons li {
  padding: 10px;
  font-size: 18px;
  color: #000;
}
#categoryButtons li:hover {
  background-color: #ccc;
}
#categoryButtons li a {
  font-size: 18px;
  color: #000;
}
#categoryButtons .active {
  background-color: #ccc;
}
</style>
