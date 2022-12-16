<template>
 <div class="wrapper">

<header class="header">
  <div class= "header__container _container" v-bind:class="{ 'icon-mobile-view': mobileNav }">
  <a class="header__logo"><img src="./assets/logo.svg" alt="growfy-logo" class="">  </a>
  <nav class="header__menu menu">
    <ul class="menu__list" v-show="!mobile">
      <li class="menu__item"><a href="" class="menu__link">Home</a></li>
      <li class="menu__item"><a href="" class="menu__link">Product</a></li>
      <li class="menu__item"><a href="" class="menu__link">Pricing</a></li>
      <li class="menu__item"><a href="" class="menu__link">Contact</a></li>
    </ul>
      <ul class="dropdown-nav" v-show="mobileNav">
        <li class="link">Home</li>
        <li class="link">Product</li>
        <li class="link">Pricing</li>
        <li class="link">Services</li>
      </ul>
   </nav>
  <div class="icon" v-on:click="toggleMobileNav" v-show="mobile">
   </div>
   <div class="header__cart cart">
    <span class="cart__text">Cart</span>
    <span class="cart__amount">0</span>
  </div>
  <a class="header__button button" href="">Get started</a>
  </div>

</header>
 <div class="main">main</div>
 <footer class="footer">footer</footer>
 </div>

</template>

<script>
/*import HelloWorld from './components/HelloWorld.vue' */

export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style>
@import url("./normalize.css");
@import url(https://fonts.googleapis.com/css?family=Poppins:300,regular,500&display=swap);

html, body { height:100%; width:100%; }
body {
  font-family: 'Poppins';
  font-weight: 300;
  color: #9C9C9C;
  background-color: #0D0D11;
}
[class*='_container'] {
  max-width: 1310px;
  margin: 0 auto;
  padding: 0 15px;
}
.wrapper {
  min-height: 100%;
  display: flex;
  flex-direction: column;
  overflow: clip;
  }
/*--------------------*/
.main {
  flex: 1 1 auto;
}
/*-----Header-----*/
 .icon {
   background-image: url();
   width: 30px;
  background-size: cover;
}
.icon-mobile-view {
  display: flex;
  justify-content: space-between;
 }
 /*.header {
  position: relative;
 } */
 .header__container {
  
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    width: 100%;
    padding: 32px 0;
    justify-content: flex-end;
    column-gap: 35px;
}
 .header__menu {
  flex: 1 1 auto;
    display: flex;
    justify-content: flex-end;
 }
 
 .menu__list {
   display: flex;
   align-items: center;
   justify-content: flex-end;
  flex-wrap: wrap;
     gap: 35px;
  }
 /*   .menu__item:not(:last-child) {
     margin: 0 35px 0 0;
 } */
 .menu__link {
  font-weight: 300;
font-size: 16px;
line-height: 26px;
display: flex;
align-items: center;
color: #FFFFFF;
  }
  .menu__link:hover {
    text-shadow: 5px 5px #558ABB;
  }
   .dropdown-nav {
    margin: 0;
    display: flex;
   flex-direction: column;
    align-items: flex-start;
    align-content: space-around;
    position: absolute;
      width: 120px;
      background-color: white;
      top: 104px;
      right: 0;
      padding: 30px 0 30 20px;
    }
    .dropdown-nav li {
      color: black;
      padding: 10px;
    }
.cart {
  display: flex;
  gap: 5px;
}
.cart__text {
  font-weight: 300;
font-size: 17.6px;
line-height: 28px;
display: flex;
align-items: center;
letter-spacing: 0.96px;
}
.cart__amount {
  background: rgba(129, 129, 139, 0.3);
  border-radius: 50%;
  font-weight: 500;
font-size: 14px;
display: flex;
align-items: center;
text-align: center;
letter-spacing: 0.96px;
height: 30px;
    width: 30px;
    justify-content: center;
 }
 .button {
font-weight: 500;
font-size: 14px;
letter-spacing: 2px;
color: #FFFFFF;
padding: 16px 30px;
background: #3D96F4;
border: 2px solid #3D96F4;
border-radius: 50px;
flex: 0 0 auto;
transition: all 0.5s;
 }
 .button:hover {
  background: #032c57;
  border: 2px solid white;
 }
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/

</style>
