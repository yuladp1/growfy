<template>
  <section class="page_feedback feedback">
    <div class="feedback__container _container">
      <div class="feedback__content">
        <div class="feedback__content-wrapper">
          <a href="" class="feedback__content-button-top button-top">testimonials</a>
          <div class="feedback__content-title content-title">
            See what our clients say
          </div>
          <div class="feedback__content-text content-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, suspendisse varius
            enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros
            dolor.
          </div>
        </div>
        <a href="" class="button">Get in touch</a>
      </div>

      <div class="feedback__items">
        <div class="feedback__item">
          <div class="feedback__item-customer">
            <img src="../assets/feedback-images/1.png" alt="" />
            <div class="feedback__item-customer-info">
              <div class="feedback__item-name">John Doe</div>
              <div class="feedback__item-job">Company Name</div>
            </div>
          </div>
          <h2 class="feedback__item-title">"I recommend this agency"</h2>
          <p class="feedback__item-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
            enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros
            dolor interdum nulla, ut commodo diam libero.
          </p>
          <div class="feedback__item-rate">
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
          </div>
        </div>
        <div class="feedback__item">
          <div class="feedback__item-customer">
            <img src="../assets/feedback-images/2.png" alt="" />
            <div class="feedback__item-customer-info">
              <div class="feedback__item-name">John Doe</div>
              <div class="feedback__item-job">Company Name</div>
            </div>
          </div>
          <h2 class="feedback__item-title">"I recommend this agency"</h2>
          <p class="feedback__item-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
            enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros
            dolor interdum nulla, ut commodo diam libero.
          </p>
          <div class="feedback__item-rate">
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
          </div>
        </div>
        <div class="feedback__item">
          <div class="feedback__item-customer">
            <img src="../assets/feedback-images/3.png" alt="" />
            <div class="feedback__item-customer-info">
              <div class="feedback__item-name">John Doe</div>
              <div class="feedback__item-job">Company Name</div>
            </div>
          </div>
          <h2 class="feedback__item-title">"I recommend this agency"</h2>
          <p class="feedback__item-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius
            enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros
            dolor interdum nulla, ut commodo diam libero.
          </p>
          <div class="feedback__item-rate">
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
            <img src="../assets/feedback-images/Star.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "SectionFeedback",
};
</script>

<style>
.page__feedback {
  padding-bottom: 96px;
}
.feedback__content {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  padding: 192px 0 64px 0;
}

.feedback__content-wrapper {
  display: flex;
  flex-direction: column;
}

.feedback__content-title,
.feedback__content-text,
.feedback__content-button-top {
  max-width: fit-content;
}

.feedback__items {
  display: flex;
  gap: 48px;
}
.feedback__item {
  padding: 64px 50px;
  background: rgba(129, 129, 139, 0.1);
  border-radius: 30px;
}
.feedback__item > *:not(:last-child) {
  margin-bottom: 34px;
}
.feedback__item:hover {
  -webkit-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  -moz-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
}
.feedback__item-customer {
  display: flex;
  gap: 16px;
}
.feedback__item-customer-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.feedback__item-name {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  color: white;
}
.feedback__item-job {
  font-weight: 300;
  font-size: 14px;
  line-height: 22px;
  display: flex;
  align-items: center;
  color: #9c9c9c;
}
.feedback__item-title {
  font-weight: 400;
  font-size: 32px;
  line-height: 45px;
  color: #ffffff;
}
.feedback__item-text {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
  color: #9c9c9c;
}
.feedback__item-rate > img:not(:last-child) {
  padding-right: 5px;
}
@media (max-width: 1080px) {
  .feedback__items {
    flex-direction: column;
  }
  .feedback__content {
    padding-top: 80px;
  }
}
@media (max-width: 690px) {
  .feedback__content {
    flex-direction: column;
    gap: 32px;
    align-content: flex-start;
    flex-wrap: wrap;
  }
  .feedback__content > a {
    align-self: flex-start;
  }
}
</style>
