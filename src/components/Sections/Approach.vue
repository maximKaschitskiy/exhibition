<script setup lang="ts">
</script>

<template>
    <section class="approach">
        <div class="approach__content">
            <h6 class="approach__content-title">
                IT подход к продаже мебели
            </h6>
            <p class="approach__content-article">
                Используя опыт e-commerce по продаже техники, мы создали инновационные цифровые продукты для управления
                мебельными предприятиями и оцифровкой всех этапов продажи продукции на заказ.
                <br>
                <br>
                Под управлением компании фабричное производство и более 10 салонов, в которых используются все наработки и
                доводятся до идеала.
            </p>
            <div class="approach__speed">
                <div class="approach__speed-card">
                    <p class="approach__speed-value">10x</p>
                    <p class="approach__speed-title">Увеличение скорости обработки первичной заявки</p>
                    <p class="approach__speed-caption">За счет внедрения в экосистему собственного конструктора
                        с автодизайном</p>
                </div>
                <div class="approach__speed-card">
                    <p class="approach__speed-value">3x</p>
                    <p class="approach__speed-title">Увеличение скорости обработки первичной заявки</p>
                    <p class="approach__speed-caption">За счет внедрения в экосистему собственного конструктора
                        с автодизайном</p>
                </div>
            </div>
        </div>
        <div class="approach__trip">
            <img src="../../assets/trip_cover.png" class="approach__trip-cover">
            <h6 class="approach__trip-title">
                Запишитесь
                на экскурсию по
                нашей экосистеме
            </h6>
            <button class="approach__button">Записаться</button>
        </div>
    </section>
</template>

<style scoped lang="scss">
.approach {
    display: flex;
    box-sizing: border-box;
    gap: 48px;

    @media only screen and (max-width: $sm) {
        flex-direction: column;
        padding: 0 12px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        flex-direction: row;
        padding: 0 12px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        flex-direction: row;
    }

    @media only screen and (min-width: $lg) {
        flex-direction: row;
    }
}

.approach__content {
    display: flex;
    justify-content: space-around;
    align-items: flex-start;
    flex-direction: column;
    gap: 24px;
}

.approach__content-title {
    color: var(--accent-2-primary, #001233);
    text-align: left;
    margin: 0;
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 22px;
        line-height: 28px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 28px;
        line-height: 36px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 36px;
        line-height: 44px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 40px;
        line-height: 48px;
    }
}


.approach__content-article {
    color: var(--light-greyscale-text-secondary, #4F5361);
    text-align: left;
    margin: 0;

    @media only screen and (max-width: $sm) {
        @include sm-caption;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-caption;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include xm-caption;
    }

    @media only screen and (min-width: $lg) {
        @include lg-caption;
    }
}

.approach__button {
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

.approach__button::after {
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

.approach__trip {
    border-radius: 32px;
    background: var(--light-greyscale-bg-dark, #F6F7F9);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    @media only screen and (max-width: $sm) {
        padding: 24px 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 24px 16px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 40px 40px 48px 40px;
    }

    @media only screen and (min-width: $lg) {
        padding: 40px 40px 48px 40px;
    }
}

.approach__trip-cover {
    height: auto;

    @media only screen and (max-width: $sm) {
        width: 161px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        width: 212px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 267px;
    }

    @media only screen and (min-width: $lg) {
        width: 310px;
    }
}

.approach__trip-title {
    color: var(--accent-2-primary, #001233);
    text-align: left;
    font-style: normal;
    font-weight: 500;
    margin: 0;
    margin-top: 22px;

    @media only screen and (max-width: $sm) {
        font-size: 18px;
        line-height: 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 24px;
        line-height: 32px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 28px;
        line-height: 36px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 36px;
        line-height: 44px;
    }
}

.approach__speed {
    width: 100%;
    box-sizing: border-box;

    @media only screen and (max-width: $sm) {
        display: flex;
        flex-direction: column;
        gap: 24px;
        justify-content: space-evenly;
        align-content: space-evenly;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto;
        gap: 0 24px;
        justify-content: space-evenly;
        justify-items: center;
        align-content: space-evenly;
        align-items: center;
    }
}

.approach__speed-value {
    color: #001233;
    font-style: normal;
    font-weight: 900;
    margin: 0;
    text-align: left;
    background-color: #1E1079;
    color: #1E1079;
    background: radial-gradient(#1E1079, #d6d2ee);
    background-repeat: no-repeat;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-background-clip: text;
    -moz-text-fill-color: transparent;

    @media only screen and (max-width: $sm) {
        font-size: 80px;
        line-height: 88px;
        background-size: 50%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 80px;
        line-height: 88px;
        background-size: 25%;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 80px;
        line-height: 88px;
        background-size: 25%;
    }

    @media only screen and (min-width: $lg) {
        font-size: 124px;
        line-height: 130px;
        background-size: 75%;
    }
}

.approach__speed-title {
    color: var(--accent-2-primary, #001233);
    font-style: normal;
    font-weight: 500;
    margin: 0;
    text-align: left;

    @media only screen and (max-width: $sm) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 18px;
        line-height: 26px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 20px;
        line-height: 28px;
    }
}

.approach__speed-caption {
    color: var(--light-greyscale-text-secondary, #4F5361);
    text-align: left;
    margin: 0;

    @media only screen and (max-width: $sm) {
        @include xs-caption;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include xs-caption;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include md-caption;
    }

    @media only screen and (min-width: $lg) {
        @include md-caption;
    }
}
</style>
