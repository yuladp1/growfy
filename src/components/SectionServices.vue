<template>
  <section class="page__services services">
    <div class="services__container _container">
      <div class="services__content">
        <a href="" class="services__content-button-top">services</a>
        <div class="services__content-title content-title">Services we offer</div>
        <div class="services__content-text content-text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, suspendisse varius enim
          in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor.
        </div>
        <a href="" class="button">All services</a>
      </div>

      <div class="services__items">
        <div class="services__item-column">
          <div class="services__item">
            <a class="services__item-icon">
              <img src="../assets/services-images/1.svg" alt="" />
            </a>
            <div class="services__item-title">Social Media Marketing</div>
            <div class="services__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit.
            </div>
          </div>
          <div class="services__item">
            <a class="services__item-icon">
              <img src="../assets/services-images/2.svg" alt="" />
            </a>
            <div class="services__item-title">Email Marketing</div>
            <div class="services__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit.
            </div>
          </div>
        </div>
        <div class="services__item-column">
          <div class="services__item">
            <a class="services__item-icon">
              <img src="../assets/services-images/3.svg" alt="" />
            </a>
            <div class="services__item-title">Paid Advertising</div>
            <div class="services__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit.
            </div>
          </div>
          <div class="services__item">
            <a class="services__item-icon">
              <img src="../assets/services-images/4.svg" alt="" />
            </a>
            <div class="services__item-title">SEO Optimization</div>
            <div class="services__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit.
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionServices",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style>
.services__container {
  display: flex;
  justify-content: space-between;
}

.services__content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}
.services__content-button-top {
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
.services__content-button-top:hover {
  background: black;
  border: 1px solid white;
  color: white;
}
.services__content-title {
  max-width: 433.31px;
}
.services__content-text {
  max-width: 491px;
}
.services__items {
  display: flex;
  flex: 0 1 47%;
  column-gap: 32px;
}
.services__item-column {
  display: flex;
  flex-direction: column;
  row-gap: 32px;
}
.services__item-column:first-child {
  margin-top: 48px;
}
.services__item {
  background: rgba(129, 129, 139, 0.1);
  padding: 55px 25px 61.41px 25px;
  align-items: flex-start;
  border-radius: 30px;
}
.services__item-icon {
  display: inline-block;
}
.services__item-icon:not(:last-child) {
  margin-bottom: 16px;
}
.services__item-title {
  font-weight: 400;
  font-size: 19.2px;
  line-height: 27px;
}
.services__item-title:not(:last-child) {
  margin-bottom: 10px;
}
.services__item-text {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  /* or 150% */

  display: flex;
  align-items: center;

  color: #81818b;
}
@media (max-width: 991.98px) {
  .services__items {
    margin-top: 20px;
  }
  .services__container {
    display: flex;
    flex-direction: column;
  }
  .services__content-title {
    font-size: 2.75rem;
  }
}

@media (max-width: 500px) {
  .services__items {
    display: flex;
    flex-direction: column;
    row-gap: 32px;
  }
}
</style>
