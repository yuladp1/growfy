<template>
  <section class="page__statistics statistics">
    <div class="statistics__wrapper _container">
      <div class="statistics__items">
        <div class="statistics__items-column">
          <div class="statistics__item">
            <div class="statistics__title content-title">1.2M+</div>
            <div class="statistics__text content-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
              enim.
            </div>
          </div>
          <div class="statistics__item">
            <div class="statistics__title content-title">1.2M+</div>
            <div class="statistics__text content-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
              enim.
            </div>
          </div>
        </div>
        <div class="statistics__items-column">
          <div class="statistics__item">
            <div class="statistics__title content-title">1.2M+</div>
            <div class="statistics__text content-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
              enim.
            </div>
          </div>
          <div class="statistics__item">
            <div class="statistics__title content-title">1.2M+</div>
            <div class="statistics__text content-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
              enim.
            </div>
          </div>
        </div>
      </div>
      <div class="statistics__image">
        <img src="../assets/statistics-images/1.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionStatistics",
};
</script>

<style>
.statistics__wrapper {
  display: flex;
  column-gap: 32px;
  flex-wrap: nowrap;
}
.statistics__items {
  display: flex;
  column-gap: 32px;
  flex-wrap: nowrap;
  flex: 0 1 58.48%;
}
.statistics__items-column {
  display: flex;
  flex-direction: column;
  gap: 32px;
  flex: 0 1 50%;
}
.statistics__item {
  padding: 38px 38px;
  background: rgba(129, 129, 139, 0.1);
  border-radius: 30px;
  flex: 0 1 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.statistics__item:hover {
  -webkit-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  -moz-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
}
.statistics__image > img {
  object-fit: cover;
  width: 100%;
}

@media (max-width: 1190px) {
  .statistics__wrapper {
    flex-direction: column;
    column-gap: 32px;
  }
  .statistics__image {
    margin-top: 32px;
  }
  .statistics__image > img {
    object-fit: cover;
    width: 50%;
  }
}
@media (max-width: 460px) {
  .statistics__items {
    display: flex;
    gap: 32px;
    flex-wrap: wrap;
    flex: 0 1 100%;
  }
  .statistics__items-column {
    display: flex;
    flex-direction: column;
    gap: 32px;
    flex: 0 1 100%;
  }
}
</style>
