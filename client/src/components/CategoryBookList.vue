<template>
  <div>
    <article id="image-grid">
      <h5>Best-selling Romance Titles</h5>
      <ul id="bookBoxes">
        <category-book-list-item :book="books[0]"></category-book-list-item>
        <category-book-list-item :book="books[1]"></category-book-list-item>
        <category-book-list-item :book="books[2]"></category-book-list-item>
        <category-book-list-item :book="books[3]"></category-book-list-item>
      </ul>
    </article>
  </div>
</template>

<script>
import CategoryBookListItem from "./CategoryBookListItem";

export default {
  name: "CategoryBookList",
  props: {
    books: {
      type: Array,
      required: true
    }
  },
  components: {
    CategoryBookListItem
  }
};
</script>

<style scoped>
#image-grid{
	width: 100%;
}
#image-grid h5{
	padding: 10px 30px;
	text-align: left;
	color: #e07517;
	font-size: 20px;
}
ul {
  padding: 10px;
  text-align: left;
  display: flex;
  align-content: flex-start;
  flex-wrap: wrap;
}
</style>
