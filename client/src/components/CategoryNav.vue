<template>
  <nav>
    <router-link to="category/classics" tag="button" id="selected">
      Classics
    </router-link>
    <router-link to="category/fantasy" tag="button">
      Fantasy
    </router-link>
    <router-link to="category/mystery" tag="button">
      Mystery
    </router-link>
    <router-link to="category/romance" tag="button">
      Romance
    </router-link>
  </nav>
</template>

<script>
export default {
  name: "CategoryNav"
};
</script>

<style scoped>
nav {
  padding: 1em;
}

#selected {
  background: darkblue;
}
</style>
