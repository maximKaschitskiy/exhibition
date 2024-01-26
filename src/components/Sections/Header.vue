<template>
  <header class="header">
    <div class="header__wrapper">
      <img src="../../assets/haier.svg" class="header__logo" alt="Haier logo" />
      <h5 class="header__title">
        Участник
        <br>
        мебель-экспо
      </h5>
      <div class="header__divider"></div>
      <div class="header__subtitle">
        <p class="header__subtitle_thin">
          стенд
        </p>
        <p class="header__subtitile_wide">
          FB020
        </p>
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
.header {
  box-sizing: border-box;

  @media only screen and (max-width: $sm) {
    padding: 0 $sm-space;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    padding: 0;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    padding: 0;
  }

  @media only screen and (min-width: $lg) {
    padding: 0;
  }
}

.header__wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  box-sizing: border-box;

  @media only screen and (max-width: $sm) {
    padding: $sm-space;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    padding: $sm-space 16px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    padding: $md-space 22px;
  }

  @media only screen and (min-width: $lg) {
    padding: $lg-space 22px;
  }
}

.header__logo {
  width: auto;

  @media only screen and (max-width: $sm) {
    height: 32px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    height: 40px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    height: 56px;
  }

  @media only screen and (min-width: $lg) {
    height: 56px;
  }
}

.header__title {
  margin: 0;
  margin-left: auto;
  color: var(--light-greyscale-text-primary, #04091D);
  text-align: right;
  font-style: normal;
  font-weight: 300;

  @media only screen and (max-width: $sm) {
    font-size: 12px;
    line-height: 14px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    font-size: 12px;
    line-height: 16px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    font-size: 16px;
    line-height: 20px;
  }

  @media only screen and (min-width: $lg) {
    font-size: 16px;
    line-height: 20px;
  }
}

.header__divider {
  width: 1px;
  background: var(--light-greyscale-dividers, #C0C2C7);
  height: 100%;

  @media only screen and (max-width: $sm) {
    height: 32px;
    margin-left: 8px;
    margin-right: 8px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    height: 40px;
    margin-left: 12px;
    margin-right: 12px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    height: 48px;
    margin-left: 16px;
    margin-right: 16px;
  }

  @media only screen and (min-width: $lg) {
    height: 48px;
    margin-left: 16px;
    margin-right: 16px;
  }
}

.header__subtitle {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}

.header__subtitle_thin {
  color: var(--light-greyscale-icons, #7B7D83);
  margin: 0;

  @media only screen and (max-width: $sm) {
    font-size: 10px;
    font-style: normal;
    font-weight: 400;
    line-height: 12px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: 14px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: 16px;
  }

  @media only screen and (min-width: $lg) {
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: 16px;
  }
}

.header__subtitile_wide {
  color: var(--light-greyscale-text-primary, #04091D);
  margin: 0;

  @media only screen and (max-width: $sm) {
    font-size: 14px;
    font-style: normal;
    font-weight: 700;
    line-height: 18px;
  }

  @media only screen and (min-width: $sm) and (max-width: $md) {
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: 26px;
  }

  @media only screen and (min-width: $md) and (max-width: $lg) {
    font-size: 28px;
    font-style: normal;
    font-weight: 700;
    line-height: 32px;
  }

  @media only screen and (min-width: $lg) {
    font-size: 28px;
    font-style: normal;
    font-weight: 700;
    line-height: 32px;
  }
}
</style>
