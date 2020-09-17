<template>
  <!-- <div class="bookBox">
    <a href="#">
      <img
        :src="require('@/assets/images/books/' + book.imageFile)"
        :alt="book.title"
      />
    </a>
    <h1>{{ book.title }}</h1>
    <h2>{{ book.author }}</h2>
    <h3>${{ (book.price / 100).toFixed(2) }}</h3>
    <button>Add to Cart</button>
    <button>Read Now</button>
  </div>-->
    
      <!-- Product image 1 start -->
      <li class="bookBlock">
        <div class="bookImage">
          <a href="#">
                <img
            :src="require('@/assets/images/books/' + book.imageFile)"
            :alt="book.title"
          />
          </a>
        </div>
        <div id="image-text" class="cate-text">
          <ul class="bookInfo">
            <li class="bookTitle">{{ book.title }}</li>
            <li class="bookAuthor">{{ book.author }}</li>
            <li class="bookPrice">${{ (book.price / 100).toFixed(2) }}</li>
          </ul>
          <ul class="bookButtons">
            <li class="addToCartButton">
              <router-link to="#" class="bookButtonLink" href="#">
                <img src="../assets/images/site/cart-logo.png" />
              </router-link>
            </li>
            <li class="readNowButton">
              <router-link to="#" class="bookButtonLink" href="#">
                <img src="../assets/images/site/read-icon.png" />
              </router-link>
            </li>
          </ul>
        </div>
      </li>
</template>

<script>
export default {
  name: "categoryBookListItem",
  props: {
    book: {
      type: Object,
      required: true
    }
  }
};
</script>
<style scoped>
#bookBoxes{
	display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
}
#bookBoxes .bookBlock{
    margin: 0px 50px 0px 50px ;
}
#image-text{
    display: flex;
    justify-content: space-between;
    padding: 5px 0px;
}
#image-text .bookInfo li{
   font-size: 14px;
   margin-right: 5px;
   text-align: left;
}
.bookButtonLink{
	width: 30px;
	height: 30px;
}
.bookButtonLink img{
	width: 100%;
}

#bookBoxes .bookBlock .bookImage{
	width: 200px;
	height: 210px;
}
#bookBoxes .bookBlock .bookImage a img{
	width: 100%;
	height: 100%;
}
.cate-text .bookAuthor{
  font-style: italic;
}
.cate-text .bookPrice{
	color: orange;
}
</style>
