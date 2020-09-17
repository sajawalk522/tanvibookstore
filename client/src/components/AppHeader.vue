<template>
  <header>
    <div id="leftheader">
      <div id="logo">
        <router-link to="/">
          <img src="../assets/images/site/bookstore-logo.png" alt="Bookstore Logo" height="100" />
        </router-link>
      </div>
    </div>
    <div id="midheader">
      <div class="flex">
        <div id="logoText">
          <router-link to="/">
            <img src="../assets/images/site/logo-text.png" alt="Wisdom Bookstore" />
          </router-link>
        </div>
        <div class="search-container">
          <header-category-dropdown></header-category-dropdown>
          <header-search-bar></header-search-bar>
        </div>
      </div>
    </div>
    <div id="rightheader"> 
      <div id="cartButton">
        <router-link to="/cart" href="cart.html">
          <img src="../assets/images/site/cart-logo.png" alt="Cart Icon" />
        </router-link>
        <div id="cartCount">1</div>
      </div>
      <div id="loginButton">Tanvi</div>
      <div id="loginButton">Login</div>
    </div>
  </header>
</template>

<script>
import HeaderSearchBar from "@/components/HeaderSearchBar";
import HeaderCategoryDropdown from "@/components/HeaderCategoryDropdown";
export default {
  name: "AppHeader",
  components: { HeaderSearchBar, HeaderCategoryDropdown },
  component: {
    HeaderSearchBar,
    HeaderCategoryDropdown
  }
};
</script>

<style scoped>
/* header seting start */
header {
  display: flex;
  justify-content: space-between;
  background-color: rgb(246, 181, 154);
  color: rgb(197, 90, 17);
  border: 1px solid #cc3599;
  padding: 8px 20px;
  align-items: center;
}
.search-container {
  display: flex;
}
/* left side header setting start  */
#logo {
  width: 120px;
  height: 120px;
}
#logo img {
  width: 100%;
  height: 100%;
}
#logoText {
  width: 445px;
  height: 72px;
  margin: 0 auto;
}
#logoText img {
  width: 100%;
}
/* left side header setting end  */
#midheader {
  text-align: center;
  display: flex;
}
#midheader .flex {
  height: 120px;
}
/* right side header setting start*/
#cartButton {
  position: relative;
  right: 15px;
}
#cartCount {
  position: absolute;
  top: -10px;
  background-color: #fc6400;
  color: #fff;
  border-radius: 100%;
  padding: 2px 5px;
  font-size: 12px;
  right: -3px;
  font-weight: bold;
}
#loginButton {
  border: 2px solid #cb6724;
  padding: 3px 18px;
  align-self: center;
  border-radius: 6px;
  font-size: 14px;
  margin-left: 14px;
  cursor: pointer;
}
#loginButton:hover{
  background:#cb6724;
  color: #111;
  border: 2px solid #111;

}
#rightheader {
  display: flex;
  align-self: flex-start;
  padding: 10px 0;
}
/* right side header setting end*/
/* header seting end */
</style>
