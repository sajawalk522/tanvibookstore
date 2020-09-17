<template>
  <footer>
    <div id="leftfooter">
      <h6>Follow us on:</h6>
      <div class="flexItem">
        <ul class="horizontal">
          <li>
            <router-link to="#" href="#">
              <img src="../assets/images/site/Picture9.png" width="32" height="32" />
            </router-link>
          </li>
          <li>
            <router-link to="#">
              <img src="../assets/images/site/Picture10.png" width="32" height="32" />
            </router-link>
          </li>
          <li>
            <router-link to="#">
              <img src="../assets/images/site/Picture11.png" width="32" height="32" />
            </router-link>
          </li>
        </ul>
      </div>
    </div>
    <div class="mid-conatainer">
      <div>
        <ul class="horizontal">
          <li>
            <router-link to="#">About</router-link>
          </li>
          <li>
            <router-link to="#" href="#">Directions</router-link>
          </li>
          <li>
            <router-link to="#">Contact Us</router-link>
          </li>
          <li>
            <router-link to="#">Help</router-link>
          </li>
        </ul>
        <p>© 2020 WisdomBookstore Inc. All Rights Reserved</p>
      </div>
    </div>
    <div id="rightfooter">
      <div class="flexItem">
        <p>For feedback/suggestions:</p>
        <p>
          <router-link to="#">Click Here</router-link>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter"
};
</script>

<style scoped>
footer {
  display: flex;
  justify-content: space-between;
  background-color: rgb(246, 181, 154);
  color: rgb(197, 90, 17);
  align-items: center;
  padding: 6px 60px;
}
footer p {
  font-size: 14px;
  color: #de7014;
}
#leftfooter {
  width: 150px;
}
#rightfooter p a {
  color: #de7014;
}
#rightfooter p {
  text-align: left;
}
#leftfooter .horizontal {
  display: flex;
  justify-content: space-around;
}
#leftfooter .horizontal li {
  padding: 5px;
}
#rightfooter p a:hover {
  color: #c55c14;
}
.mid-conatainer .horizontal li a:hover {
  color: #c55c14;
}
#leftfooter h6 {
  color: #de7014;
  font-size: 14px;
  text-align: center;
}
.mid-conatainer,
#rightfooter {
  line-height: 1.5;
}
.mid-conatainer h4 {
  font-weight: bold;
  font-size: 18px;
}
.mid-conatainer p {
  font-size: 12px;
}
.mid-conatainer .horizontal {
  display: flex;
}
.mid-conatainer .horizontal li {
  display: flex;
  border-right: 3px solid #de7014;
  padding: 0 12px;
}
.mid-conatainer .horizontal li:last-child {
  border: unset;
}
.mid-conatainer .horizontal li a {
  color: #de7014;
  font-weight: 600;
  font-size: 14px;
}
</style>
