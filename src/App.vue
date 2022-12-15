<template>
 <div class="wrapper">

<header class="header">header</header>
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html, body { height:100%; width:100%; }
body {
  font-family: 'Poppins';
  font-weight: 300;
  color: #9C9C9C;
  background-color: 0D0D11S;
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
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/

</style>
