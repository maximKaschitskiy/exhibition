<script setup lang="ts">
</script>

<template>
    <section class="calculate">
            <div class="calculate__content">
                <p class="calculate__title">Открой студию кухонной мебели с показателем продаж до 125 000 рублей с
                    квадратного метра
                </p>
                <p class="caclulate__subtitle">Рассчитайте стоимость открытия салона под Ваши условия
                </p>
                <button class="calculate__button">Рассчитать</button>
            </div>
    </section>
</template>

<style scoped lang="scss">
.calculate {
    box-sizing: border-box;
    display: flex;

    @media only screen and (max-width: $sm) {
        padding: 0 12px
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

.calculate__content {
    display: flex;
    width: 100%;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    box-sizing: border-box;
    z-index: 3;
    position: relative;
    border-radius: 24px;
    overflow: hidden;
    padding: 184px 16px 48px 16px;
    background-repeat: no-repeat;

    @media only screen and (max-width: $xs) {
        background-position: top 0 right 0;
        background-size: auto 50%;
        padding: 184px 16px 48px 16px;
        background-image: url('../../assets/kitchen_sm.png');
    }

    @media only screen and (min-width: $xs) and (max-width: $sm) {
        background-position: top 0;
        background-size: cover;
        padding: 184px 16px 48px 16px;
        background-image: url('../../assets/kitchen_sm.png');
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        background-size: cover;
        padding: 80px 24px 80px 24px;
        background-image: url('../../assets/kitchen_md.png');
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        background-size: cover;
        background-image: url('../../assets/kitchen_md.png');
        padding: 136px 32px 136px 36px;
    }

    @media only screen and (min-width: $lg) {
        background-size: cover;
        background-image: url('../../assets/kitchen_lg.png');
        padding: 196px 48px 208px 48px;
    }
}

.calculate__title {
    margin: 0;
    text-align: left;
    color: var(--light-greyscale-bg-light, #FFF);
    z-index: 3;

    @media only screen and (max-width: $sm) {
        @include sm-title;
        width: 100%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include md-title;
        width: 528px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include md-title;
        width: 488px;
    }

    @media only screen and (min-width: $lg) {
        @include lg-title;
        width: 715px;
    }
}

.caclulate__subtitle {
    text-align: left;
    margin: 0;
    color: var(--light-greyscale-bg-light, #FFF);
    z-index: 3;

    @media only screen and (max-width: $sm) {
        @include xs-caption;
        width: 100%;
        margin-top: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-caption;
        width: 300px;
        margin-top: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include md-caption;
        width: 300px;
        margin-top: 20px;
    }

    @media only screen and (min-width: $lg) {
        @include lg-caption;
        width: 376px;
        margin-top: 24px;
    }
}

.calculate__button {
    background: var(--light-greyscale-bg-light, #FFF);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    border-radius: 32px;
    color: var(--light-greyscale-text-primary, #04091D);
    z-index: 3;

    @media only screen and (max-width: $sm) {
        @include sm-button-text;
        @include sm-button-space;
        margin-top: 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-button-text;
        @include lg-button-space;
        margin-top: 32px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include sm-button-text;
        @include lg-button-space;
        margin-top: 32px;
    }

    @media only screen and (min-width: $lg) {
        @include lg-button-text;
        @include lg-button-space;
        margin-top: 40px;
    }
}

.calculate__button::after {
    content: '';
    background-image: url('../../assets/icon_arrow.svg');
    background-size: contain;

    @media only screen and (max-width: $sm) {
        width: 16px;
        height: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        width: 16px;
        height: 16px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 16px;
        height: 16px;
    }

    @media only screen and (min-width: $lg) {
        width: 24px;
        height: 24px;
    }
}

.calculate__content::before {
    content: '';
    width: 100%;
    height: 100%;
    z-index: 2;
    box-sizing: border-box;
    position: absolute;
    top: 0;
    left: 0;

    @media only screen and (max-width: $sm) {
        background: linear-gradient(348deg, #1F107C 0%, rgba(0, 0, 0, 0.10) 100%);
        opacity: 0.32;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        background: linear-gradient(332deg, #1F107C 0%, rgba(0, 0, 0, 0.10) 67.22%);
        opacity: 0.32;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        background: linear-gradient(332deg, #1F107C 0%, rgba(0, 0, 0, 0.10) 67.22%);
        opacity: 0.32;
    }

    @media only screen and (min-width: $lg) {
        background: linear-gradient(332deg, #1F107C 0%, rgba(0, 0, 0, 0.10) 67.22%);
        opacity: 0.32;
    }
}

.calculate__content::after {
    content: '';
    width: 100%;
    height: 100%;
    z-index: 2;
    box-sizing: border-box;
    position: absolute;
    top: 0;
    left: 0;
    @media only screen and (max-width: $sm) {
        background: linear-gradient(0, #000 49.97%, rgba(0, 0, 0, 0.00) 99.86%);
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        background: linear-gradient(-270deg, #000 63.76%, rgba(0, 0, 0, 0.00) 100%);   
        background-position: left 0 top 0;
        background-size: 50% auto;
        background-repeat: no-repeat;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        background: linear-gradient(-270deg, #000 63.76%, rgba(0, 0, 0, 0.00) 100%);   
        background-position: left 0 top 0;
        background-size: 50% auto;
        background-repeat: no-repeat;
    }

    @media only screen and (min-width: $lg) {
        background: linear-gradient(-270deg, #000 63.76%, rgba(0, 0, 0, 0.00) 100%);   
        background-position: left 0 top 0;
        background-size: 50% auto;
        background-repeat: no-repeat;
    }
}
</style>
