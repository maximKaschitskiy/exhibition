<template>
  <Carousel v-bind="settings" :breakpoints="breakpoints">
    <Slide :key="a2">
      <div class="cards-bar__wrapper">
        <img class="cards-bar__icon" src="../../assets/card_pc.png">
        <div class="cards-bar__content">
          <p class="cards-bar__card-title">Бесплатная
            <br>CRM система
          </p>
          <p class="cards-bar__card-subtitle">Подробнее</p>
        </div>
      </div>
    </Slide>
    <Slide :key="b2">
      <div class="cards-bar__wrapper">
        <img class="cards-bar__icon" src="../../assets/card_ai.png">
        <div class="cards-bar__content">
          <p class="cards-bar__card-title">ИИ, который делает
            <br>проекты кухонь 24/7
          </p>
          <p class="cards-bar__card-subtitle">Подробнее</p>
        </div>
      </div>
    </Slide>
    <Slide :key="c2">
      <div class="cards-bar__wrapper">
        <img class="cards-bar__icon" src="../../assets/card_building.png">
        <div class="cards-bar__content">
          <p class="cards-bar__card-title">Бесплатный
            <br>конструктор
          </p>
          <p class="cards-bar__card-subtitle">Подробнее</p>
        </div>
      </div>
    </Slide>
    <template #addons>
      <Pagination />
    </template>
  </Carousel>
</template>

<script scoped>
import { defineComponent } from 'vue'
import { Carousel, Pagination, Slide } from 'vue3-carousel'

import 'vue3-carousel/dist/carousel.css'

export default defineComponent({
  name: 'BCarousel',
  components: {
    Carousel,
    Slide,
    Pagination,
  },
  data: () => ({
    settings: {
      itemsToShow: 1,
      snapAlign: 'center',
    },
    breakpoints: {
      741: {
        itemsToShow: 3,
        snapAlign: 'center',
      },
    },
  }),
})
</script>


<style lang="scss">
.carousel__prev {
  box-sizing: content-box;
  border: 5px solid white;
}

.carousel__next {
  box-sizing: content-box;
  border: 5px solid white;
}

.carousel__pagination-button {
  width: 8px;
  height: 8px;
  margin: 0 4px;
  border-radius: 4px;
  background: var(--light-greyscale-dividers, #C0C2C7);
}

.carousel {
  z-index: 3;

  @media only screen and (max-width: $sm) {
    transform: translate(0, -25%);
    padding: 0 16px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    padding: 0 24px;
    transform: translate(0, -50%);
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    padding: 0 32px;
    transform: translate(0, -50%);
  }

  @media only screen and (min-width: $lg) {
    padding: 0 48px;
    transform: translate(0, -50%);
  }
}

.carousel__viewport {
  box-sizing: border-box;

  @media only screen and (max-width: $sm) {
    overflow: hidden;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {}

  @media only screen and (min-width: $md) and (max-width: $lg) {}

  @media only screen and (min-width: $lg) {
    overflow: visible;
  }
}

.cards-bar__wrapper {
  display: flex;
  border-radius: 16px;
  border: 1px solid var(--light-greyscale-disabled-bg, #F2F3F4);
  background: var(--light-greyscale-white, #FFF);
  box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.04);
  justify-content: flex-start;
  box-sizing: border-box;
  gap: 12px;
  width: 100%;

  @media only screen and (max-width: $sm) {
    padding: 12px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    padding: 18px 12px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    padding: 28px 12px;
  }

  @media only screen and (min-width: $lg) {
    padding: 32px 12px;
  }
}

.cards-bar__card {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: row;
  margin-left: 8px;
  margin-right: 8px;
  flex: 1 auto;
  border-radius: 24px;
  border: 1px solid var(--light-greyscale-disabled-bg, #F2F3F4);
  background: var(--light-greyscale-white, #FFF);
  box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.04);
}

.cards-bar__card-title {
  margin: 0;
  text-align: left;
  color: var(--accent-2-primary, #001233);
  font-style: normal;

  @media only screen and (max-width: $sm) {
    font-size: 14px;
    line-height: 20px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    font-size: 14px;
    line-height: 20px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    font-size: 20px;
    line-height: 28px;
    font-weight: 500;
  }

  @media only screen and (min-width: $lg) {
    font-size: 24px;
    line-height: 32px;
    font-weight: 500;
  }
}

.cards-bar__card-subtitle {
  text-align: left;
  margin: 0;
  font-style: normal;
  font-weight: 400;
  color: var(--light-greyscale-disabled-text, #6B6C72);

  @media only screen and (max-width: $sm) {
    font-size: 12px;
    line-height: 18px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    font-size: 12px;
    line-height: 18px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    font-size: 16px;
    line-height: 24px;
  }

  @media only screen and (min-width: $lg) {
    font-size: 16px;
    line-height: 24px;
  }
}

.cards-bar__icon {
  width: auto;
  align-self: center;

  @media only screen and (max-width: $sm) {
    height: 47px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    height: 47px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    height: 63px;
  }

  @media only screen and (min-width: $lg) {
    height: 94px;
  }
}

.cards-bar__content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;

  @media only screen and (max-width: $sm) {
    gap: 8px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    gap: 8px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    gap: 8px;
  }

  @media only screen and (min-width: $lg) {
    gap: 12px;
  }
}

.carousel__pagination-button {
  margin: 0;
  padding: 0;
  width: 16px;
  height: 2px;
  border-radius: 4px;
  background: var(--light-greyscale-stroke, #E6E6E8);
}

.carousel__pagination-item {
  margin: 0;
  margin: 0 2px;
}

.carousel__pagination-button::after {
  display: none;
}

.carousel__pagination-button--active {
  border-radius: 4px;
  background: var(--light-greyscale-dividers, #C0C2C7);
}

.carousel__pagination {
  /* display: none; */
  margin-top: 8px;
}

.carousel__slide {
  box-sizing: border-box;

  @media only screen and (max-width: $sm) {

  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    flex: 1;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    flex: 1;
  }

  @media only screen and (min-width: $lg) {
    flex: 1;
  }
}

.carousel__track {
  margin: 0;

  @media only screen and (max-width: $sm) {
    gap: 32px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    gap: 16px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    gap: 12px;
  }

  @media only screen and (min-width: $lg) {
    gap: 16px;
  }
}

.carousel__viewport {
  box-sizing: border-box;
}
</style>
