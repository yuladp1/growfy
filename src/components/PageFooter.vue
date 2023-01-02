<template>
  <footer class="page__footer footer _container">
    <div class="footer__wrapper">
      <div class="footer__menu1">
        <div class="footer__menu1-logo"><img src="../assets/logo.svg" alt="" /></div>
        <div class="footer__menu-text">
          Growfy is a template highly suitable for modern marketing agencies, digital
          studios, startups and businesses. The design is made in the dark style, which
          makes the site memorable and you can easily adapt it to your brand.
        </div>
        <div class="footer__menu1-icons">
          <a href=""> <img src="../assets/footer-images/1.svg" alt="" /> </a>
          <a href=""> <img src="../assets/footer-images/2.svg" alt="" /> </a>
          <a href=""> <img src="../assets/footer-images/3.svg" alt="" /> </a>
          <a href=""> <img src="../assets/footer-images/4.svg" alt="" /> </a>
          <a href=""> <img src="../assets/footer-images/5.svg" alt="" /> </a>
        </div>
      </div>
      <div class="footer__menu-list">
        <ul>
          <li class="footer__menu-items-title">Pages</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
        </ul>
      </div>

      <div class="footer__menu-list">
        <ul>
          <li class="footer__menu-items-title">Utility pages</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
          <li class="footer__menu-item">Instructions</li>
        </ul>
      </div>

      <div class="footer__menu4">
        <span class="footer__menu-items-title">Subscribe to our newsletter</span>
        <p class="footer__menu-text">Lorem ipsum dolor sit am consectetur adipiscing</p>
        <div class="footer__buttons">
          <a href="" class="button button-dark">Enter your email</a>
          <a href="" class="button">Subscribe</a>
        </div>
      </div>
    </div>
    <div class="footer__copyright">
      <span class="copyright__symbol">c</span>
      <span class="copyright__year">2022</span>
    </div>
  </footer>
</template>

<script>
export default {
  name: "PageFooter",
};
</script>
<style>
footer {
  margin-top: 160px;
}
.footer__wrapper {
  display: flex;
  padding: 160px 0 183px 0;
  gap: 64px;
  justify-content: space-between;
}

.footer__menu1 {
  display: flex;
  flex-direction: column;
  flex-basis: 377px;
}
.footer__menu1 > *:not(:last-child) {
  padding-bottom: 32px;
}
.footer__menu-text {
  font-weight: 300;
  font-size: 16px;
  line-height: 24px;
}
.footer__menu1-icons {
  display: flex;
  gap: 16px;
}
.footer__menu-list {
  display: flex;
  flex-basis: 139px;
}
.footer__menu-items-title {
  display: inline-block;
  font-weight: 500;
  font-size: 20px;
  line-height: 24px;
  letter-spacing: 1px;
  color: #ffffff;
  margin-bottom: 31px;
}
.footer__menu-item {
  font-weight: 300;
  font-size: 16px;
  line-height: 26px;
}
.footer__menu-item:hover {
  color: white;
  text-decoration: underline;
}
.footer__menu-item:not(:last-child) {
  margin-bottom: 24.39px;
}
.footer__menu4 {
  flex-basis: 377px;
}
.footer__menu4 > *:not(:last-child) {
  margin-bottom: 32px;
}
.footer__buttons {
  display: flex;
  gap: 16px;
}
.footer__copyright {
  display: flex;
  gap: 5px;
  align-items: center;
  justify-content: center;
  border-top: 1px solid rgba(129, 129, 139, 0.2);
  padding: 46px 0;
}
.copyright__symbol {
  display: flex;
  width: 10px;
  height: 10px;
  padding: 1px;
  border: 1px solid rgba(129, 129, 139, 0.2);
  border-radius: 50%;
  justify-content: center;
  align-items: center;
  font-size: 10px;
}
.copyright__year {
  font-weight: 300;
  font-size: 14px;
  line-height: 22px;
}

@media (max-width: 1180px) {
  .footer__wrapper {
    flex-wrap: wrap;
    justify-content: center;
    gap: 80px;
  }
  .footer__wrapper {
    padding: 100px 0 100px 0;
  }
}
@media (max-width: 800px) {
  .footer__wrapper {
    gap: 80px;
  }
  .footer__buttons {
    flex-wrap: wrap;
  }
  .start__buttons > a,
  .footer__buttons > a {
    flex: 0 1 100%;
    text-align: center;
  }
}
</style>
