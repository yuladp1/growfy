<template>
  <section class="page__clients clients">
    <div class="clients__wrapper _container">
      <h2 class="clients__title">TRUSTED BY startups and large enterprises</h2>
      <div class="clients__items">
        <div class="clients__item">
          <img src="../assets/clients-images/1.svg" alt="" />
        </div>
        <div class="clients__item">
          <img src="../assets/clients-images/2.svg" alt="" />
        </div>
        <div class="clients__item">
          <img src="../assets/clients-images/3.svg" alt="" />
        </div>
        <div class="clients__item">
          <img src="../assets/clients-images/4.svg" alt="" />
        </div>
        <div class="clients__item">
          <img src="../assets/clients-images/5.svg" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionClients",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style>
.page__clients {
  padding: 192px 0 160px 0;
}
.clients__title {
  font-weight: 300;
  font-size: 0.875;
  line-height: 1.5714;
  letter-spacing: 1px;
  text-align: center;
  text-transform: uppercase;
  margin-bottom: 24px;
}
.clients__items {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
.clients__item {
  flex: 0 1 20%;
  min-width: 210px;
}
@media (max-width: 991.98px) {
  .page__clients {
    padding: 80px 0 80px 0;
  }
}
</style>
