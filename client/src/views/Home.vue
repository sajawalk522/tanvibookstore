<template>
  <div id="home">
    <!-- <p>
      Welcome to another bookstore &ndash; a client-side application written in
      Vue. It includes a home-page view and a category-page view. The reason
      these are views and not proper pages is because this is a single-page
      application. The Vue router allows you to navigate between pages as you
      would in a traditional web app. Take some time and explore the code.
    </p> -->
    <home-category-list></home-category-list>
  </div>
</template>

<script>
import HomeCategoryList from "@/components/HomeCategoryList";
export default {
  name: "Home",
  components: {
    HomeCategoryList
  }
};
</script>

<style scoped>
#home {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

p {
  font-family: "Proza Libre", sans-serif;
  line-height: 1.3;
  width: 300px;
  margin: 10px;
}
</style>
