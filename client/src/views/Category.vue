<template>
  <div class="category-primary">
    <!-- <category-nav></category-nav> -->
    <CategorySideNav></CategorySideNav>
    <category-book-list :books="books"> </category-book-list>
  </div>
</template>

<script>
// import CategoryNav from "@/components/CategoryNav";
import CategoryBookList from "@/components/CategoryBookList";
import CategorySideNav from "@/components/CategorySideNav";

export default {
  name: "category",
  components: {
    CategoryBookList,
    CategorySideNav
  },
  data: function() {
    return {
      books: [
        {
          bookId: 1001,
          title: "The Iliad",
          imageFile: "the-iliad.gif",
          author: "Homer",
          price: 699,
          isPublic: true
        },
        {
          bookId: 1002,
          title: "The Brothers Karamazov",
          imageFile: "the-brothers-karamazov.gif",
          author: "Fyodor Dostoyevski",
          price: 1399,
          isPublic: false
        },
        {
          bookId: 1003,
          title: "Little Dorrit",
          imageFile: "little-dorrit.gif",
          author: "Charles Dickens",
          price: 599,
          isPublic: true
        },
        {
          bookId: 1004,
          title: "Moby Dick",
          imageFile: "moby-dick.gif",
          author: "Herman Melville",
          price: 699,
          isPublic: true
        }
      ]
    };
  }
};
</script>

<style scoped>
.category-primary{
  display: flex;
  margin: 10px 0;
}
</style>
