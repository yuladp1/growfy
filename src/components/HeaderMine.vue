<template>
  <header class="header">
    <div
      class="header__container _container"
      v-bind:class="{ 'icon-mobile-view': mobileNav }"
    >
      <a class="header__logo"
        ><img src="../assets/logo.svg" alt="growfy-logo" class="" />
      </a>
      <transition name="slide-fade" appear>
        <nav class="header__menu menu">
          <ul class="menu__list" v-show="!mobileNav">
            <li class="menu__item"><a href="" class="menu__link">Home</a></li>
            <li class="menu__item"><a href="" class="menu__link">Product</a></li>
            <li class="menu__item"><a href="" class="menu__link">Pricing</a></li>
            <li class="menu__item"><a href="" class="menu__link">Contact</a></li>
          </ul>
        </nav>
      </transition>

      <div class="header__cart cart">
        <span class="cart__text">Cart</span>
        <span class="cart__amount">0</span>
      </div>
      <a class="header__button button" href="">Get started</a>
      <div class="icon" v-on:click="toggleMobileNav" v-show="mobileNav"></div>
    </div>

    <transition name="slide-fade">
      <ul class="dropdown-nav" v-show="isBurgerClicked">
        <li class="dropdown-nav-link">Home</li>
        <li class="dropdown-nav-link">Product</li>
        <li class="dropdown-nav-link">Pricing</li>
        <li class="dropdown-nav-link">Services</li>
      </ul></transition
    >
  </header>
</template>

<script>
export default {
  name: "HeaderMain",
  data() {
    return {
      scrollPosition: null,
      isBurgerClicked: false,
      mobileNav: true,
      windowWidth: null,
    };
  },
  mounted() {
    this.checkScreen();
  },
  created() {
    window.addEventListener("resize", this.checkScreen);
  },
  methods: {
    toggleMobileNav() {
      this.isBurgerClicked = !this.isBurgerClicked;
    },
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 798) {
        this.mobileNav = true;
        return;
      } else {
        this.mobileNav = false;
        this.isBurgerClicked = false;
        return;
      }
    },
  },
};
</script>

<style>
/*-----Header-----*/
.icon {
  background-image: url("../assets/burger-menu.png");
  width: 30px;
  height: 30px;
  background-size: cover;
}
.icon-mobile-view {
  display: flex;
  justify-content: space-between;
}
.header {
  position: fixed;
  width: 100%;
  height: 116px;
  padding: 32px 0;
  display: flex;
  flex-direction: column;
  background: rgba(0, 0, 0, 0.8);
  z-index: 100;
}
.header__container {
  display: flex;
  align-items: center;
  width: 100%;
  margin-top: 32px;
  justify-content: flex-end;
  column-gap: 35px;
}
.header__menu {
  height: 100%;
  flex: 1 1 auto;
  display: flex;
  justify-content: flex-end;
}

.menu__list {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 25px;
}

.menu__link {
  font-weight: 300;
  font-size: 1rem;
  line-height: 26px;
  display: flex;
  align-items: center;
  color: #ffffff;
  -webkit-transition: all 150ms ease-in-out;
  transition: all 150ms ease-in-out;
  padding: 0 10px;
}
.menu__link:hover {
  -webkit-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  -moz-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
}

.dropdown-nav {
  margin: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  align-content: space-around;
  position: fixed;
  width: 100%;
  top: 90px;
  overflow: auto;
  background: rgba(0, 0, 0, 0.93);
  z-index: 1;
  font-weight: 500;
  height: 50vh;
  padding-top: 30px;
  margin-top: 25px;
}
.dropdown-nav-link {
  color: white;
  font-size: 2rem;
  padding: 20px;
  width: 100%;
  text-align: center;
}
.dropdown-nav-link:hover {
  -webkit-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  -moz-box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
  box-shadow: 0px 5px 10px 2px rgba(235, 240, 244, 0.2) inset;
}
.cart {
  display: flex;
  gap: 5px;
}
.cart__text {
  font-weight: 300;
  font-size: 1.1rem;
  line-height: 1.59;
  display: flex;
  align-items: center;
  letter-spacing: 0.96px;
}
.cart__amount {
  background: rgba(129, 129, 139, 0.3);
  border-radius: 50%;
  font-weight: 500;
  font-size: 0.875rem;
  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: 0.96px;
  height: 30px;
  width: 30px;
  justify-content: center;
}
@media (max-width: 991.98px) {
  .menu__list {
    column-gap: 25px;
  }
}
@media (max-width: 850px) {
  .header__container {
    column-gap: 20px;
  }
  .menu__list {
    column-gap: 10px;
  }
}
@media (max-width: 560px) {
  .header__container {
    column-gap: 10px;
  }
  .header__logo {
    width: 40px;
    overflow: hidden;
  }
}

@media (max-width: 375px) {
  .header__container > .header__button {
    font-size: 10px;
    padding: 16px 10px;
  }
}
</style>
