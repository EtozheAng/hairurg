<script setup></script>

<template>
  <header class="header js-header">
    <div class="header__wrapper wrapper">
      <a class="header__logo" href="/" title="Главная">
        <img
          class="header__logo-img"
          width="119"
          height="26"
          src="https://scantronicsystems.com/local/templates/scantronicsystems/img/logo.svg"
          alt="Скантроник Системс"
        />
      </a>
      <nav class="header__menu">
        <ul
          class="header__menu-list caps"
          itemscope
          itemtype="https://www.schema.org/SiteNavigationElement"
        >
          <li class="header__menu-item" itemprop="name">
            <a class="header__menu-link link" itemprop="url" href="/about/">
              О компании
            </a>
          </li>
          <li class="header__menu-item" itemprop="name">
            <a class="header__menu-link link" itemprop="url" href="/catalog/">
              Продукция
            </a>
          </li>
          <li class="header__menu-item" itemprop="name">
            <a
              class="header__menu-link link"
              itemprop="url"
              href="/technologies/"
            >
              Технологии
            </a>
          </li>
          <li class="header__menu-item" itemprop="name">
            <a class="header__menu-link link" itemprop="url" href="/news/">
              Новости
            </a>
          </li>
          <li class="header__menu-item" itemprop="name">
            <a class="header__menu-link link" itemprop="url" href="/contacts/">
              Контакты
            </a>
          </li>
        </ul>
      </nav>
      <ul class="header__nav">
        <li class="header__nav-item header__nav-item--lang">
          <a class="nav-link" href="/en/"> En </a>
        </li>
        <li class="header__nav-item">
          <button
            id="btn-menu-modal-auth"
            class="nav-link"
            title="Вход в личный кабинет менеджера"
          >
            <svg class="nav-link__icon" width="24" height="24">
              <!-- <use
                href="/local/templates/scantronicsystems/img/icons.svg#auth"
                xlink:href="/local/templates/scantronicsystems/img/icons.svg#auth"
              ></use> -->
            </svg>
          </button>
          <div
            id="top-menu-modal-container"
            class="top-menu-modal-container"
          ></div>
        </li>
        <li class="header__nav-item">
          <button
            id="btnTopMenuSearch"
            class="nav-link js-search-open"
            title="Поиск"
          >
            <svg class="nav-link__icon" width="24" height="24">
              <!-- <use
                href="/local/templates/scantronicsystems/img/icons.svg#search"
                xlink:href="/local/templates/scantronicsystems/img/icons.svg#search"
              ></use> -->
            </svg>
          </button>
          <div id="TopMenuSearchPanel" class="top-menu-search-panel"></div>
        </li>
      </ul>
      <button class="header__btn btn fos-topmenu-btn fos-modal-header-btn">
        Оставить заявку
      </button>
      <div
        id="ajax-add-answer"
        class="ajax-add-answer"
        style="display: block"
      ></div>
      <div
        id="ajax-add-popUpSuccess"
        class="ajax-add-popup-success"
        style="display: block"
      ></div>
      <button
        class="header__burger nav-link nav-link--burger js-menu-toggle"
        title="Меню"
      ></button>
    </div>
  </header>
</template>

<style scoped>
.header {
  z-index: 3;
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  background: #f9f9f9;
}

.header__wrapper {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  padding-top: 15rem;
  padding-bottom: 14rem;
}

@media (max-width: 800.98px) {
  .header__wrapper {
    padding-top: 16rem;
    padding-bottom: 16rem;
  }
}

.header__logo {
  -webkit-transition: opacity 0.3s ease;
  -o-transition: opacity 0.3s ease;
  transition: opacity 0.3s ease;
}

.header__logo:hover {
  opacity: 0.5;
}

.header__logo-img {
  display: block;
  width: 119rem;
  height: auto;
}

@media (max-width: 800.98px) {
  .header__logo-img {
    width: 137rem;
  }
}

.header__menu {
  margin-left: 55rem;
}

@media (max-width: 800.98px) {
  .header__menu {
    display: none;
  }
}

.header__menu-list {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  margin: -21rem;
  padding: 0;
  list-style: none;
}

.header__menu-item {
  margin: 21rem;
}

.header__menu-link {
  display: inline-block;
}

.header__nav {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  margin: -1rem -1rem -1rem auto;
  padding: 0;
  list-style: none;
}

.header__nav-item {
  position: relative;
  margin: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
}

.header__nav-sublist {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  padding: 0;
  list-style: none;
}

.header__nav-lang.is-active + .header__nav-sublist {
  display: block;
}

.header__nav-subitem {
  margin-top: 2rem;
}

.header__btn {
  margin-left: 9rem;
}

@media (max-width: 800.98px) {
  .header__btn {
    position: fixed;
    right: 0;
    border: 1px solid rgba(255, 255, 255, 0.1);
    bottom: 28rem;
    margin-left: 0;
  }
}

.header__burger {
  display: none;
  margin-left: 2rem;
}

@media (max-width: 800.98px) {
  .header__burger {
    display: -webkit-inline-box;
    display: -ms-inline-flexbox;
    display: inline-flex;
  }
}

.menu {
  display: none;
  z-index: 2;
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100%;
  -webkit-transform: translateY(-100%);
  -ms-transform: translateY(-100%);
  transform: translateY(-100%);
  background: #f9f9f9;
  -webkit-transition: -webkit-transform 0.3s ease;
  -o-transition: transform 0.3s ease;
  transition: transform 0.3s ease;
  transition: transform 0.3s ease, -webkit-transform 0.3s ease;
}
</style>
