<template>
  <div >
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <nav>
      <input type="checkbox" id="check">
      <label for="check" class="checkbtn">
        <img src="../assets/square.png">
      </label>
      <!-- <label class="logo-title">Minha Logo</label> -->
      <img src="../assets/favoriteInactive.png" id="heart">
      <ul>
        <li><a class="active" href="#">Início</a></li>
        <li><a href="#">Móveis</a></li>
        <li><a href="#">Construção</a></li>
        <li><a href="#">Ferramentas</a></li>
        <li><a href="#">Brinquedos</a></li>
        <li><a href="#">Tecnologias</a></li> 
      </ul>
    </nav>
    <div>
      <section class="leading">
          <p class="leading-bigtext">Hello</p>
          <p class="leading-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vitae semper quam. Praesent lobortis tellus quis erat condimentum, a bibendum tortor volutpat.</p>
        </section>
        <section class="cards">
          <article>
            <img class="article-img" src="http://placekitten.com/305/205" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
          <article>
            <img class="article-img" src="http://placekitten.com/320/220" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
          <article>
            <img class="article-img" src="http://placekitten.com/330/240" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
          <article>
            <img class="article-img" src="http://placekitten.com/280/250" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
          <article>
            <img class="article-img" src="http://placekitten.com/310/210" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
          <article>
            <img class="article-img" src="http://placekitten.com/430/240" alt=" " />
            <h1 class="article-title">
              Title of article
            </h1>
          </article>
        </section>
    </div>
  </div>
</template>

<script>

export default {
  
  
}
</script>

<style scoped>
nav {
	background: #A2ABE9;
	height: 90px;
	width: 100%;
  padding: 0;
	margin: 0;
}
.logo-title {
	color: white;
	font-size: 35px;
	line-height: 80px;
	padding: 0 100px;
	font-weight: bold;
}
nav ul {
	float: right;
	margin-right: 20px;
}
nav ul li {
	display: inline-block;
	line-height: 80px;
	margin: 0 5px;
  font-size: 14px;
}
nav ul li a {
	color: white;
	font-size: 17px;
	padding: 7px 13px;
	border-radius: 3px;
	text-transform: uppercase;
}
a.active, a:hover {
	background: #1d075f;
	transition: .5s;
}
.checkbtn {
	font-size: 30px;
	color: white;
	float: right;
	line-height: 80px;
	margin-right: 40px;
	cursor: pointer;
	display: none;
}
#check {
	display: none;
}
#heart{
  margin: 30px
}

@media (max-width: 1063px){
	.checkbtn {
		display: block;
    margin-top: 1%;
	}
	ul{
		position: fixed;
		width: 100%;
		height: 100vh;
		background: #1d075f;
    opacity: 0.95;
		top: 80px;
		left: -100%;
		text-align: center;
		transition: all .5s;
	}
	nav ul li{
		display: block;
		margin: 50px 0;
		line-height: 30px;
	}
	nav ul li a {
		font-size: 20px;
	}
	a:hover, a.active {
		background: none;
		color: #C69CBF;
	}
	#check:checked ~ ul {
		left: 0;
    z-index: 1;
	}
}

/* @media (max-width: 952px){
	label.logo{
		font-size: 30px;
		padding-left: 50px;
	}
	nav ul li a{
		font-size: 16px;
	}
} */

@media (max-width: 858px){
	.checkbtn {
		display: block;
    margin-top: 1%;
	}
	ul{
		position: fixed;
		width: 100%;
		height: 100vh;
		background: #1d075f;
		top: 80px;
		left: -100%;
		text-align: center;
		transition: all .5s;
	}
	nav ul li{
		display: block;
		margin: 50px 0;
		line-height: 30px;
	}
	nav ul li a {
		font-size: 20px;
	}
	a:hover, a.active {
		background: none;
		color: #5434af;
	}
	#check:checked ~ ul {
		left: 0;
    z-index: 1;
	}
}

@media (max-width: 558px){
  .checkbtn {
		display: block;
    margin-top: 3%;
	}
}

header {
  display: flex;
  align-items: center;
}

@media (min-width: 700px) {
 .leading {
    display: flex;
    align-items: center;
  }
}


/* Grid styles -------------------------------------------------*/
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  grid-gap: 30px;
}

.leading {
  height: 240px;
  width: 100vw;
  margin-bottom: 30px;
  padding: 30px;
  color: white;
  background: url('https://cdn.glitch.com/a5121e34-96b3-4a70-8227-040c51e64fae%2Fcat.jpg?1509635989509') center #333 no-repeat;
  background-size: cover;
  color: white;
  text-shadow: 0px 0px 5px #000;
}

.leading-bigtext {
  margin-right: 60px;
  font-weight: bold;
  font-size: 24vw;
}

@media (min-width: 700px) {
  .leading-bigtext {
    font-size: 140px;
  }
}

.leading-text {
  max-width: 900px;
  font-size: 1.2em;
  line-height: 1.4em;
}

.cards {
  max-width: 960px;
  margin: 0 auto 30px;
}

article {
  position: relative;
}

.article-img {
  height: 200px;
  width: 100%;
  object-fit: cover;
}

.article-title {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 10px;
  background-color: rgba(255, 255, 255, 0.2);
}

</style>
