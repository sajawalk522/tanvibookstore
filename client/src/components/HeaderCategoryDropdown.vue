<template>
  <!-- Dropdown start -->
  <div class="browse-container">
    <div class="container-cat">
      <div id="dropdown-main">
        <h1>Browse Categories</h1>
        <ul id="categoryDropdownList">
          <router-link to="../category/classics" tag="li">Classics</router-link>
          <router-link to="../category/fantasy" tag="li">Fantasy</router-link>
          <router-link to="../category/mystery" tag="li">Mystery</router-link>
          <router-link to="../category/romance" tag="li">Romance</router-link>
        </ul>
      </div>
    </div>
    <div class="image-browse">
      <img src="../assets/images/site/bars.jpg" />
    </div>
  </div>
  <!-- Dropdown end -->
</template>

<script>
export default {
  name: "HeaderCategoryDropdown"
};
</script>

<style scoped>
.browse-container {
  display: flex;
  align-items: center;
  margin: 0 11px 0 0;
  cursor: pointer;
}
.browse-container .container-cat {
  border: 1px solid #ce7b42;
  padding: 6px 15px;
  border-right: unset;
}
.browse-container .container-cat p {
  font-size: 16px;
}
.image-browse {
  background-image: linear-gradient(to bottom left, #de495e 49%, #efbf52);
  padding: 6px 5px;
}
.image-browse img {
  width: 18px;
  position: relative;
  top: 0;
}
#dropdown-main ul {
  display: none;
  position: absolute;
  background-color: #fff;
  padding: 10px 10px;
  width: 157px;
  left: -16px;
  z-index: 1;
  top: 22px;
  text-align: left;
}
#dropdown-main ul li {
  padding: 5px 0px;
  color: #000;
}
#dropdown-main ul li:hover {
  color: #cb6724;
}
.browse-container:hover #categoryDropdownList {
  display: block;
}
#dropdown-main {
  display: flex;
  justify-content: center;
  position: relative;
  font-size: 14px;
}
</style>
