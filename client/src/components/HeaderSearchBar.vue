<template>
  <!-- Search bar start -->
  <form id="searchForm">
    <input type="text" placeholder="Enter keyword, title or author " />
    <input type="image" :src="require('../assets/images/site/search.jpg')" alt="image" />
  </form>
  <!-- Search bar end -->
</template>

<script>
export default {
  name: "HeaderSearchBar"
};
</script>

<style scoped>
#searchForm {
  display: flex;
  justify-content: center;
}
#searchForm input {
  font-size: 14px;
  color: #d6d4d4;
}
#searchForm input[type="text"] {
  background-color: #f2f2f2;
  border: 1px solid #ce7b42;
  padding: 6px 8px;
  width: 300px;
  color: #969595;
  border-right: unset;
}
#searchForm input[type="image"] {
  background-color: #4bc7ca;
  padding: 5px 8px;
  width: 24px;
}
#searchForm input:focus {
  outline: none;
}
</style>
