<template>
 <div class="wrapper">

<HeaderMine />
 <div class="main">main</div>
 <footer class="footer">footer</footer>
 </div>

</template>

<script>
import HeaderMine from './components/HeaderMine.vue'

export default {
  name: 'App',
  components: {
    HeaderMine
    
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
.main {
  flex: 1 1 auto;
}

/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/

</style>
