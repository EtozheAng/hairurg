<script setup></script>

<template>
  <header class="header js-header">
    <div class="header__wrapper wrapper">
      <a class="header__logo" href="/" title="Главная">
        <img
          class="header__logo-img"
          width="119"
          height="26"
          src="../assets/Header-logo.svg"
          alt="Скантроник Системс"
        />
      </a>
    </div>
  </header>
  <!-- <header class="header js-header">
    <div class="header__wrapper wrapper">
      <a class="header__logo" href="/" title="Главная">
        <img
          class="header__logo-img"
          width="119"
          height="26"
          src="../assets/Header-logo.svg"
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
              <use
                href="/local/templates/scantronicsystems/img/icons.svg#auth"
                xlink:href="/local/templates/scantronicsystems/img/icons.svg#auth"
              ></use>
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
              <use
                href="/local/templates/scantronicsystems/img/icons.svg#search"
                xlink:href="/local/templates/scantronicsystems/img/icons.svg#search"
              ></use>
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
  </header> -->
</template>

<style scoped>
.wrapper {
  width: 100%;
  max-width: 1392rem;
  margin-right: auto;
  margin-left: auto;
  padding-right: 24rem;
  padding-left: 24rem;
}
</style>
