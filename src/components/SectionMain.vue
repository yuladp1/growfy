<template>
  <section class="page__main">
    <div class="page__main-wrapper _container">
      <div class="page__main-content">
        <div class="page__main-content-title content-title">
          Marketing solutions that grow your business.
        </div>
        <div class="page__main-content-text content-text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, suspendisse varius enim
          in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor.
        </div>
        <div class="page__main-content-buttons">
          <a href="" class="button">Our services</a>
          <a href="" class="button button-dark">Contact us</a>
        </div>
      </div>

      <div class="page__main-images">
        <div class="page__main-images-column">
          <img
            class="page__main-images-image1"
            src="../assets/main-images/1.jpg"
            alt=""
          />
          <img
            class="page__main-images-image2"
            src="../assets/main-images/2.jpg"
            alt=""
          />
        </div>
        <div class="page__main-images-column">
          <img
            class="page__main-images-image3"
            src="../assets/main-images/3.jpg"
            alt=""
          />
          <img
            class="page__main-images-image4"
            src="../assets/main-images/4.jpg"
            alt=""
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionMine",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style>
.page__main {
  margin-top: 160px;
}
.page__main-wrapper {
  margin-top: 65px;
  display: flex;
  justify-content: space-between;
}
.page__main-content {
  display: flex;
  flex-direction: column;
  flex: 0 1 50%;
  margin-top: 124px;
  position: relative;
}
.page__main-content::before {
  content: "";
  background: url("../assets/decor.png");
  position: absolute;
  width: 122px;
  top: -20px;
  left: -30px;
  height: 122px;
}

.content-title:not(:last-child) {
  margin-bottom: 32px;
}

.content-text:not(:last-child) {
  margin-bottom: 32px;
}
.page__main-content-buttons {
  display: flex;
  column-gap: 32px;
}

.page__main-images {
  display: flex;
  column-gap: 9.61%;
  justify-content: center;
}
.page__main-images img {
  max-width: 100%;
}
.page__main-images-column {
  display: flex;
  flex-direction: column;
  row-gap: 32px;
}
.page__main-images-image1,
.page__main-images-image4 {
  border-radius: 378px;
}
.page__main-images-image2 {
  border-radius: 241.906px 241.906px 0px 241.906px;
}
.page__main-images-image3 {
  border-radius: 241.906px 0px 241.906px 241.906px;
}
@media (max-width: 991.98px) {
  .content-title {
    font-size: 2.75rem;
  }
}
@media (max-width: 850px) {
  .page__main-content-buttons {
    column-gap: 10px;
    margin: 0 auto;
  }
  .page__main-content-buttons a {
    font-size: 1.3rem;
    padding: 10px 20px;
    letter-spacing: 0.1px;
  }
}
@media (max-width: 767.98px) {
  .page__main-content {
    margin: 0 0 20px 0;
  }
  .content-title {
    font-size: 2rem;
  }
  .page__main-wrapper {
    flex-direction: column;
    align-items: center;
  }
}
@media (max-width: 400px) {
  .page__main-content-buttons {
    column-gap: 10px;
    margin: 0 auto;
  }
}
</style>
