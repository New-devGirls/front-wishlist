<template>
  <div id="app" class="content">
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
    <router-view/>
  </div>
</template>

<style >
@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;1,100;1,200;1,300;1,400;1,500;1,600&display=swap");

#app{
  font-family: "Montserrat", sans-serif;
  font-size: 15px;

}
* {
	padding: 0;
	margin: 0;
	text-decoration: none;
	list-style: none;
	box-sizing: border-box;
  vertical-align:baseline;
  list-style:none;
  border:0;
}
/* .content{
  width: 100px;
  height: 100px;
  margin: 0 auto;
} */

</style>
