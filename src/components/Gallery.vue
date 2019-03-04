<template>
<v-container grid-list-xs grid-list-md fluid>
  <div>
    <!-- directive -->
    <v-layout row wrap class="images" v-viewer="{movable: false, toolbar:false}">
    <v-flex xs12 pa-5 class="npm3" >
		<span class="section-title">גלרייה</span>
		</v-flex>
    <!-- cart -->
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/cart/1.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/cart/2.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs12 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/cart/3.jpg')">
    </div>
    </v-flex>
     </v-flex>
<!-- d4000 -->
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/d4000/d4000-0.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/d4000/d4000-1.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs12 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/d4000/d4000-2.jpg')">
    </div>
    </v-flex>
<!-- d4000b -->
    <v-flex xl2 xs12 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/d4000b/d4000-0.jpg')">
    </div>
    </v-flex>
<!-- h1 -->
    <v-flex xl2 xs12 md2>
    <div class="img-box">
      <img class="article-img"  :src="require('@/assets/H1/h1-0.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H1/h1-1.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H1/h1-2.jpg')">
    </div>
    </v-flex>
<!-- h3 -->
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H3/h3-0.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H3/h3-1.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs12 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H3/h3-2.jpg')">
    </div>
    </v-flex>
<!-- H4 -->
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H4/h4-0.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
      <img class="article-img" :src="require('@/assets/H4/h4-1.jpg')">
    </div>
    </v-flex>
<!-- h5 -->
    <v-flex xl2 xs12 md2>
    <div class="img-box">
        <img class="article-img" :src="require('@/assets/H5/h5-0.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
        <img class="article-img" :src="require('@/assets/H5/h5-1.jpg')">
    </div>
    </v-flex>
    <v-flex xl2 xs6 md2>
    <div class="img-box">
        <img class="article-img" :src="require('@/assets/H5/H5-H4.jpg')">
    </div>
    </v-flex>
    </v-layout>
  </v-container>
  </div>

</template>

<script>

  export default {
    data() {
  
     
    }
  }

</script> 

<style scoped>
	.img-box {
		overflow: hidden;
		transition: all 0.2s ease-out;
		box-shadow: -15px 10px 30px -10px #00000099;
		height: 95%;
	}
  	.article-img:hover {
		-webkit-transform: scale(1.05);
		-ms-transform: scale(1.05);
		transform: scale(1.05);
		transition: all 0.2s ease;
		cursor: pointer;
	}
.article-img {
	width: 100%;
	height: 200px;
	transition: all 0.2s ease-out;
    object-fit: cover;
	}
</style>