<template>
  <section class="page__news news">
    <div class="page__news-wrapper _container">
      <div class="news__content-wrapper">
        <div class="news__content">
          <a href="" class="news__content-button-top button-top">Blog</a>
          <div class="news__content-title content-title">Read our articles & news</div>
          <div class="news__content-text content-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
            enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros
            dolor interdum nulla, ut commodo diam libero.
          </div>
        </div>
        <a href="" class="button">All Posts</a>
      </div>

      <div class="news__items">
        <div class="news__item">
          <div class="news__item-image">
            <img src="../assets/news-images/1.png" alt="" />
            <div class="news__item-image-label">Social Media</div>
          </div>
          <div class="news__item-content-wrapper">
            <div class="news__item-date">August 28, 2022</div>
            <div class="news__item-title">How to Use Social Proof in Marketing</div>
            <div class="news__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit viverra sit semper lorem.
            </div>
            <div class="news__item-link">Read now</div>
          </div>
        </div>

        <div class="news__item">
          <div class="news__item-image">
            <img src="../assets/news-images/2.png" alt="" />
            <div class="news__item-image-label">SEO</div>
          </div>
          <div class="news__item-content-wrapper">
            <div class="news__item-date">August 28, 2022</div>
            <div class="news__item-title">
              Make a great first impression with these titles
            </div>
            <div class="news__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit viverra sit semper lorem.
            </div>
            <div class="news__item-link">Read now</div>
          </div>
        </div>
        <div class="news__item">
          <div class="news__item-image">
            <img src="../assets/news-images/3.png" alt="" />
            <div class="news__item-image-label">Strategy</div>
          </div>
          <div class="news__item-content-wrapper">
            <div class="news__item-date">August 28, 2022</div>
            <div class="news__item-title">How to Grab Your Reader’s Attention</div>
            <div class="news__item-text">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit lobortis arcu enim
              urna adipiscing praesent velit viverra sit semper lorem.
            </div>
            <a class="news__item-link">Read now</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionNews",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style>
.page__news {
  padding: 96px 0 96px 0;
}
.page__news-wrapper {
  display: flex;
  flex-direction: column;
}
.news__content-wrapper {
  display: flex;
  justify-content: space-between;
  padding-bottom: 64px;
}

.news__content {
  display: flex;
  flex-direction: column;
}
.news__content-button-top {
  max-width: fit-content;
}
.news__content-wrapper > a {
  align-self: flex-end;
}
.news__items {
  display: flex;
  gap: 48px;
}
.news__item {
  flex: 0 1 33.333%;
  background: rgba(129, 129, 139, 0.1);
  border-radius: 24px;
}

.news__item-image {
  position: relative;
}

.news__item-image-label {
  position: absolute;
  left: 0;
  bottom: 0;
  font-weight: 300;
  font-size: 14px;
  line-height: 22px;
  color: #ffffff;
  background: rgba(129, 129, 139, 0.5);
  border-radius: 0px 10px 0px 0px;
  padding: 9px 10px;
}

.news__item-image > img {
  width: 100%;
  object-fit: cover;
  border-top-left-radius: 24px;
  border-top-right-radius: 24px;
}
.news__item-content-wrapper {
  padding: 26px 29px 40px 26px;
}
.news__item-date {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  display: flex;
  align-items: center;
  color: rgba(129, 129, 139, 0.9);
}
.news__item-title {
  font-weight: 400;
  font-size: 19.2px;
  line-height: 27px;
  display: flex;
  align-items: center;
  color: #ffffff;
  padding: 20px 0 30px 0;
}
.news__item-text {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  display: flex;
  align-items: center;
}
.news__item-link {
  font-weight: 300;
  font-size: 14px;
  line-height: 22px;
  display: flex;
  align-items: center;
  color: #3d96f4;
  padding-top: 21px;
}
.news__item-link:hover {
  text-decoration: underline;
}
@media (max-width: 690px) {
  .news__content-wrapper {
    flex-direction: column;
    gap: 32px;
  }
  .news__content-wrapper > a {
    align-self: flex-start;
  }
}
@media (max-width: 1080px) {
  .news__items {
    flex-wrap: wrap;
  }
  .news__item {
    flex: 0 1 100%;
  }
}
</style>
