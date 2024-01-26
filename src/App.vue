<script setup lang="ts">
import Header from './components/Sections/Header.vue';
import Calculate from './components/Sections/Calculate.vue';
import BCarousel from './components/Sections/BCarousel.vue';
import Benefit from './components/Sections/Benefit.vue';
import Conditions from './components/Sections/Conditions.vue';
import Ecosystem from './components/Sections/Ecosystem.vue';
import Proposal from './components/Sections/Proposal.vue';
import Escort from './components/Sections/Escort.vue';
import Pluses from './components/Sections/Pluses.vue';
import Approach from './components/Sections/Approach.vue';
import Plans from './components/Sections/Plans.vue';
import Footer from './components/Sections/Footer.vue';
</script>

<template>
  <Header class="section__header"></Header>
  <Calculate class="section__calculate"></Calculate>
  <BCarousel class="section__carousel"></BCarousel>
  <Benefit class="section__benefit"></Benefit>
  <Conditions class="section__conditions"></Conditions>
  <Ecosystem class="section__ecosystem"></Ecosystem>
  <Proposal class="section__proposal"></Proposal>
  <Escort class="section__escort"></Escort>
  <Pluses class="section__pluses"></Pluses>
  <Approach class="section__approach"></Approach>
  <Plans class="section__plans"></Plans>
  <Footer class="section__footer"></Footer>
</template>

<style lang="scss">
body {
  background: var(--light-greyscale-bg-light, #FFF);
  justify-content: center;
  align-items: flex-start;
  height: max-content;
  box-sizing: border-box;
  /* min-width: 100vw; */
  /* width: 100%; */
  min-width: auto;
  /* max-width: 100vw; */
}

#app {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  width: 100%;
  max-width: 100%;
}

@media only screen and (max-width: $sm) {
  .section__header {
    width: 100%;
  }

  .section__calculate {
    width: 100%;
    margin-top: 4px;
  }

  .section__cards-bar {
    width: 100%;
  }

  .section__carousel {
    width: 100%;
    overflow: hidden;
  }

  .section__benefit {
    width: 100%;
    margin-top: 40px;
  }

  .section__conditions {
    margin-top: 64px;
    width: 100%;
  }

  .section__ecosystem {
    margin-top: 64px;
    width: 100%;
  }

  .section__proposal {
    margin-top: 64px;
    width: 100%;
  }

  .section__escort {
    margin-top: 64px;
    width: 100%;
  }

  .section__pluses {
    margin-top: 64px;
    width: 100%;
  }

  .section__approach {
    margin-top: 64px;
    width: 100%;
  }

  .section__plans {
    margin-top: 64px;
    width: 100%;
  }

  .section__footer {
    margin-top: 64px;
    width: 100%;
  }
}


@media only screen and (min-width: $sm) and (max-width: $md) {
  .section__header {
    width: 100%;
  }

  .section__calculate {
    width: 100%;
    margin-top: 4px;
  }

  .section__cards-bar {
    width: 100%;
  }

  .section__carousel {
    width: 100%;
    overflow: hidden;
  }

  .section__benefit {
    width: 100%;
    margin-top: 40px;
  }

  .section__conditions {
    margin-top: 64px;
    width: 100%;
  }

  .section__ecosystem {
    margin-top: 64px;
    width: 100%;
  }

  .section__proposal {
    margin-top: 64px;
    width: 100%;
  }

  .section__escort {
    margin-top: 64px;
    width: 100%;
  }

  .section__pluses {
    margin-top: 64px;
    width: 100%;
  }

  .section__approach {
    margin-top: 64px;
    width: 100%;
  }

  .section__plans {
    margin-top: 64px;
    width: 100%;
  }

  .section__footer {
    margin-top: 64px;
    width: 100%;
  }
}

@media only screen and (min-width: $md) and (max-width: $lg) {

  .section__header {
    width: $md;
  }

  .section__calculate {
    width: $md;
    margin-top: 2px;
  }

  .section__carousel {
    width: $md;
    margin-top: 42px;
    overflow: hidden;
  }

  .section__benefit {
    width: $md;
    margin-top: 100px;
  }

  .section__conditions {
    width: $md;
    margin-top: 100px;
  }

  .section__ecosystem {
    width: $md;
    margin-top: 100px;
  }

  .section__proposal {
    width: $md;
    margin-top: 100px;
  }

  .section__escort {
    width: $md;
    margin-top: 100px;
  }

  .section__pluses {
    width: $md;
    margin-top: 100px;
  }

  .section__approach {
    width: $md;
    margin-top: 100px;
  }

  .section__plans {
    width: $md;
    margin-top: 100px;
  }

  .section__footer {
    width: 100%;
    margin-top: 100px;
  }
}

@media only screen and (min-width: $lg) {
  .section__header {
    width: $lg;
  }

  .section__calculate {
    width: $lg;
    margin-top: 6px;
  }

  .section__carousel {
    width: $lg;
    overflow: hidden;
  }

  .section__benefit {
    width: $lg;
    margin-top: 42px;
  }

  .section__conditions {
    width: $lg;
    margin-top: 128px;
  }

  .section__ecosystem {
    width: $lg;
    margin-top: 128px;
  }

  .section__proposal {
    width: $lg;
    margin-top: 152px;
  }

  .section__escort {
    width: $lg;
    margin-top: 128px;
  }

  .section__pluses {
    width: $lg;
    margin-top: 128px;
  }

  .section__approach {
    width: $lg;
    margin-top: 144px;
  }

  .section__plans {
    width: $lg;
    margin-top: 128px;
  }

  .section__footer {
    width: 100%;
    margin-top: 128px;
  }
  
}
</style>
