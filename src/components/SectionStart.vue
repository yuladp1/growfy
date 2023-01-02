<template>
  <section class="page__start _container start">
    <div class="start__wrapper">
      <div class="start__content">
        <div class="start__title">Ready to start scaling your business now?</div>
        <div class="start__text">
          Lorem ipsum dolor sit am consectetur adipiscing varius enim in eros.
        </div>
      </div>
      <div class="start__buttons">
        <a href="" class="button">Our services</a>
        <a href="" class="button button-dark">Contact us</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionStart",
};
</script>
<style>
.page__start {
  width: 100%;
}
.start__wrapper {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  background: rgba(129, 129, 139, 0.1);
  border-radius: 30px;
  padding: 52px 40px;
  margin: 96px 0;
}

.start__content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  justify-items: center;
  flex-basis: 348px;
}
.start__title {
  font-weight: 400;
  font-size: 32px;
  line-height: 45px;
  display: flex;
  align-items: center;
  text-align: center;
  color: #ffffff;
}
.start__title:not(:last-child) {
  margin-bottom: 16px;
}
.start__text {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  text-align: center;
}
.start__buttons {
  display: flex;
  gap: 32px;
  align-items: center;
  padding: 20px;
}
@media (max-width: 500px) {
  .start__buttons {
    flex-wrap: wrap;
  }
}
@media (max-width: 1000px) {
  .start__wrapper {
    margin: 0 0;
  }
}
</style>
