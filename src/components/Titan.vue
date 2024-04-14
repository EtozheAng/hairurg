<template>
  <header>
    <div class="container">
      <div class="header">
        <button class="header-close">
          <svg
            width="32"
            height="32"
            viewBox="0 0 32 32"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M7 7L25 25"
              stroke="black"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M7 25L25 7"
              stroke="black"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
        <div class="header-logo">
          <img
            class="header-logo__img"
            src="https://titan.dev.rutego.ru/local/templates/titan/images/logo.svg"
            alt="TITAN - Производство пластиковой тары в СПб"
            title="TITAN - Производство пластиковой тары в СПб"
          />
        </div>
        <nav class="header-menu">
          <ul class="top-menu">
            <li class="top-menu__item">
              <a href="/catalog/">КАТАЛОГ</a>
            </li>
            <li class="top-menu__item">
              <a href="/about/">О КОМПАНИИ</a>
            </li>
            <li class="top-menu__item">
              <a href="/press-form/">ПРЕСС-ФОРМЫ</a>
            </li>
            <li class="top-menu__item">
              <a href="/contacts/">КОНТАКТЫ</a>
            </li>
          </ul>
        </nav>
        <div class="header-contacts">
          <div class="header-contacts__phone">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
            >
              <path
                d="M18.9994 14.4765V17.1862C19.0005 17.4377 18.9488 17.6867 18.8479 17.9172C18.7469 18.1477 18.5988 18.3546 18.413 18.5247C18.2273 18.6947 18.008 18.8242 17.7693 18.9048C17.5305 18.9854 17.2775 19.0153 17.0265 18.9927C14.2415 18.6907 11.5664 17.7409 9.21601 16.2197C7.02929 14.8329 5.17534 12.9827 3.7858 10.8003C2.25627 8.44389 1.30442 5.76107 1.00735 2.96915C0.98473 2.71938 1.01447 2.46764 1.09468 2.22996C1.17489 1.99229 1.30381 1.77389 1.47323 1.58866C1.64265 1.40343 1.84885 1.25544 2.07872 1.15411C2.30858 1.05278 2.55707 1.00032 2.80837 1.00009H5.52347C5.96269 0.995773 6.3885 1.151 6.72152 1.43683C7.05455 1.72267 7.27207 2.11961 7.33354 2.55366C7.44814 3.42084 7.66067 4.27229 7.96707 5.09177C8.08883 5.41507 8.11519 5.76642 8.043 6.1042C7.97082 6.44198 7.80313 6.75203 7.5598 6.99761L6.41041 8.14473C7.69877 10.406 9.57482 12.2784 11.8406 13.5642L12.99 12.4171C13.2361 12.1742 13.5467 12.0069 13.8852 11.9348C14.2236 11.8628 14.5757 11.8891 14.8996 12.0106C15.7207 12.3164 16.5739 12.5285 17.4428 12.6429C17.8824 12.7048 18.2839 12.9258 18.5709 13.2639C18.858 13.6019 19.0105 14.0335 18.9994 14.4765Z"
                stroke="black"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <a href="tel:+7 (812) 317-11-32 ">+7 (812) 317-11-32 </a>
          </div>
          <div class="header-contacts__email">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="16"
              viewBox="0 0 20 16"
              fill="none"
            >
              <path
                d="M19 2.75C19 1.7875 18.19 1 17.2 1H2.8C1.81 1 1 1.7875 1 2.75M19 2.75V13.25C19 14.2125 18.19 15 17.2 15H2.8C1.81 15 1 14.2125 1 13.25V2.75M19 2.75L10 8.875L1 2.75"
                stroke="black"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <a href="mailto:info@titanupak.ru">info@titanupak.ru</a>
          </div>
        </div>
        <div class="header-feedback">
          <button data-fancybox data-src="#callback-popup-call">
            Отправить запрос
          </button>
        </div>
      </div>
      <div class="header-mobile">
        <div class="header-logo">
          <img
            class="header-logo__img"
            src="https://titan.dev.rutego.ru/local/templates/titan/images/logo.svg"
            alt="TITAN - Производство пластиковой тары в СПб"
            title="TITAN - Производство пластиковой тары в СПб"
          />
        </div>
        <button class="header-mobile-burger">
          <svg
            width="33"
            height="22"
            viewBox="0 0 33 22"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M32 11H1M32 1H1M32 21H1"
              stroke="black"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  /* width: 100vw; */
  position: relative;
}

.header {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  align-items: center;
  padding-bottom: 10px;
}
.header-contacts {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.header-contacts__email,
.header-contacts__phone {
  display: flex;
  gap: 11px;
  font-size: 18px;
  line-height: 1;
}
.header-contacts__email a,
.header-contacts__phone a {
  font-weight: 500;
  color: #464646;
}
.header-contacts__phone a {
  color: #000;
  font-weight: 800;
}
.header-close {
  display: none;
  position: absolute;
  top: 15px;
  right: 15px;
}
.header-feedback button {
  color: #fff;
  border-radius: 33px;
  background-color: #000;
  font-weight: 500;
  text-transform: uppercase;
  transition: all 0.3s;
  font-size: 16px;
  padding: 15px 15px;
}
.header-feedback button:hover,
.header-feedback button:active,
.header-feedback button:focus {
  scale: 1.05;
}
.header-mobile {
  display: none;
  position: relative;
  justify-content: space-between;
}
.header-mobile-content {
  position: absolute;
  top: 0;
  right: 0;
  background-color: red;
  z-index: 10;
}
@media (max-width: 1200px) {
  .header-menu {
    flex: 1 0 100%;
    order: 1;
  }
}
@media (max-width: 992px) {
  .header {
    display: none;
    padding: 0 12px 20px;
  }
  .header-mobile {
    display: flex;
  }
  .header.active {
    display: block;
    position: absolute;
    top: 0;
    right: 0;
    background-color: #fff;
    z-index: 10;
    box-shadow: -2px 2px 5px 8px rgba(0, 0, 0, 0.11);
  }
  .header-feedback {
    text-align: center;
  }
  .header-logo img {
    height: 65px;
  }
  .header-menu {
    margin-bottom: 25px;
  }
  .header-contacts {
    margin-bottom: 25px;
  }
  .header-contacts__email,
  .header-contacts__phone {
    justify-content: center;
  }
  .header .top-menu {
    border-radius: 40px;
    flex-direction: column;
    gap: 40px;
  }
  .header-close {
    display: block;
  }
}
@media (max-width: 480px) {
  .header {
    width: 100%;
  }
  .header-mobile {
    padding: 0 5px 0;
  }
}
.top-menu {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
  padding: 13px 25px;
  border-radius: 85px;
  border: 2px solid #d5e0e2;
}
.top-menu__item {
  transition: all 0.3s;
}
.top-menu__item a {
  color: #464646;
  font-size: 16px;
  font-weight: 500;
  line-height: 1;
}
.top-menu__item:hover,
.top-menu__item:active,
.top-menu__item:focus {
  scale: 1.05;
}
.top-menu__item.active a {
  color: #000;
}
@media (max-width: 1200px) {
  .top-menu {
    padding: 10px 30px;
  }
}
</style>
