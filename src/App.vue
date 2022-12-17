<template>
  <div class="wrapper">
    <HeaderMine />
    <SectionMine />
    <footer class="footer">footer</footer>
  </div>
</template>

<script>
import HeaderMine from "./components/HeaderMine.vue";
import SectionMine from "./components/SectionMain.vue";

export default {
  name: "App",
  components: {
    HeaderMine,
    SectionMine,
  },
};
</script>

<style>
@import url("./normalize.css");
@import url(https://fonts.googleapis.com/css?family=Poppins:300,regular,500&display=swap);

html,
body {
  height: 100%;
  width: 100%;
}
body {
  font-family: "Poppins";
  font-weight: 300;
  color: #9c9c9c;
  background-color: #0d0d11;
}
[class*="_container"] {
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
  color: #ffffff;
  padding: 16px 30px;
  background: #3d96f4;
  border: 2px solid #3d96f4;
  border-radius: 50px;
  flex: 0 0 auto;
  transition: all 0.5s;
}
.button-dark {
  font-weight: 500;
  font-size: 14px;
  letter-spacing: 2px;
  color: #ffffff;
  padding: 16px 30px;
  background: rgba(129, 129, 139, 0.2);
  border: 2px solid rgba(129, 129, 139, 0.2);
  border-radius: 50px;
  flex: 0 0 auto;
  transition: all 0.5s;
  background: rgba(129, 129, 139, 0.2);
}
.button:hover {
  background: #032c57;
  border: 2px solid white;
}
.button-dark:hover {
  background: #98bfe9;
  border: 2px solid white;
}
/*--------------------*/

/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
</style>
