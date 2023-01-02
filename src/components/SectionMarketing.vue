<template>
  <section class="page__marketing marketing">
    <div class="marketing__wrapper _container">
      <div class="marketing__images">
        <div class="marketing__images-container">
          <img
            class="marketing__images-image1"
            src="../assets/marketing-images/1.png"
            alt=""
          />
        </div>
        <div class="marketing__images-container">
          <img
            class="marketing__images-image2"
            src="../assets/marketing-images/2.png"
            alt=""
          />
        </div>
      </div>
      <div class="marketing__content">
        <a href="" class="marketing__content-button-top button-top">why choose us</a>
        <div class="marketing__content-title content-title">
          We help great brands scale with content marketing.
        </div>
        <div class="marketing__content-text content-text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, suspendisse varius enim
          in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor.
        </div>
        <ul class="marketing__content-list">
          <li class="marketing__list-item">This is some text inside of a div.</li>
          <li class="marketing__list-item">This is some text inside of a div.</li>
          <li class="marketing__list-item">This is some text inside of a div.</li>
          <li class="marketing__list-item">This is some text inside of a div.</li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "SectionMarketing",
};
</script>

<style>
.marketing {
  padding: 175px 0 192px 0;
}
.marketing__wrapper {
  display: flex;
  align-items: flex-start;
}
.marketing__images {
  display: flex;
  align-items: flex-end;
  flex: 0 1 50%;
}
.marketing__images-container {
  width: 100%;
}
.marketing__images-image1 {
  width: 100%;
  position: relative;
  z-index: 2;
}
.marketing__images::after {
  content: "";
  background: url("../assets/decor.png");
  position: absolute;
  width: 122px;
  left: -10px;
  height: 122px;
}
.marketing__content {
  padding-left: 64px;
  display: flex;
  flex-direction: column;
  align-self: center;
  flex: 0 1 50%;
}
.marketing__content-list {
  padding: 34px 0 0 0;
}
.marketing__content-list > *:not(:last-child) {
  margin-bottom: 16px;
}
.marketing__list-item {
  font-weight: 300;
  font-size: 16px;
  line-height: 32px;
  padding-left: 40px;
  position: relative;
}

.marketing__list-item::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  background-image: url("../assets/marketing-images/list-decoration.svg");
  background-position: left;
  width: 32px;
  height: 32px;
}
.marketing__content-button-top {
  display: block;
  width: fit-content;
}
@media (max-width: 767.98px) {
  .marketing__wrapper {
    flex-direction: column-reverse;
    gap: 30px;
  }
  .marketing {
    padding: 100px 0 100px 0;
  }
  .marketing__content {
    padding-left: 0;
  }
}
</style>
