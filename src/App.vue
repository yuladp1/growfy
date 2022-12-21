<template>
  <div class="wrapper">
    <HeaderMine />
    <SectionMine />
    <SectionClients />
    <SectionServices />
    <SectionMarketing />
    <SectionStatistics />
    <SectionFeedback />
    <SectionNews />
    <SectionStart />
    <PageFooter />
  </div>
</template>

<script>
import HeaderMine from "./components/HeaderMine.vue";
import SectionMine from "./components/SectionMain.vue";
import SectionClients from "./components/SectionClients.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionMarketing from "./components/SectionMarketing.vue";
import SectionStatistics from "./components/SectionStatistics.vue";
import SectionFeedback from "./components/SectionFeedback.vue";
import SectionNews from "./components/SectionNews.vue";
import SectionStart from "./components/SectionStart.vue";
import PageFooter from "./components/PageFooter.vue";
export default {
  name: "App",
  components: {
    HeaderMine,
    SectionMine,
    SectionClients,
    SectionServices,
    SectionMarketing,
    SectionStatistics,
    SectionFeedback,
    SectionNews,
    SectionStart,
    PageFooter,
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
  background: rgba(129, 129, 139, 0.2);
  border: 2px solid rgba(129, 129, 139, 0.2);
}
.button:hover {
  background: #032c57;
  border: 2px solid white;
}
.button-dark:hover {
  background: #01070e;
  border: 2px solid white;
}
.content-title {
  font-weight: 500;
  font-size: 3.2rem;
  line-height: 1.1718;
  color: white;
  max-width: 520px;
}
.content-text {
  font-weight: 300;
  font-size: 1.125rem;
  line-height: 1.5;
  max-width: 491px;
}
.button-top {
  color: #9c9c9c;
  font-weight: 300;
  font-size: 10.8px;
  line-height: 17px;
  letter-spacing: 2px;
  text-transform: uppercase;
  padding: 11px 19px;
  border: 1px solid rgba(129, 129, 139, 0.2);
  border-radius: 12px;
  transition: all 0.5s;
  display: inline-block;
  margin-bottom: 19px;
}
.button-top:hover {
  background: black;
  border: 1px solid white;
  color: white;
}
/*--------------------*/

/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
/*--------------------*/
</style>
