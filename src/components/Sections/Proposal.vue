<script setup lang="ts">
</script>

<template>
    <section class="proposal">
        <div class="proposal__wrapper">
            <p class="proposal__title">
                От заявки клиента
                <br>до проекта - 5 минут
            </p>
            <p class="proposal__subtitle">За счет ИИ, работающего в связке с собственным конструктором, время
                обработки заявки сократилось в 10 раз!
                <br><br>
                Посмотрите видео как это работает
            </p>
            <video class="proposal__video" loop autoplay>
                <source src="https://zov.kitchen/_nuxt/new.79e37475.mp4" type="video/mp4">
            </video>
            <button class="proposal__button">Демо-квиз</button>
        </div>
    </section>
</template>

<style scoped lang="scss">
.proposal {
    box-sizing: border-box;
    padding: 0 12px;
}

.proposal__wrapper {
    box-sizing: border-box;
    width: 100%;
    z-index: 3;
    position: relative;
    background: linear-gradient(332deg, #193782 0%, rgba(0, 0, 0, 0.10) 67.22%), #000;
    border-radius: 32px;

    @media only screen and (max-width: $sm) {
        padding: 32px 16px 20px 16px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-between;
        height: max-content;
        box-sizing: border-box;
        z-index: 3;
        position: relative;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 32px 24px 24px 24px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-between;
        height: max-content;
        box-sizing: border-box;
        z-index: 3;
        position: relative;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 36px 32px;
        display: grid;
        grid-template-columns: auto max-content;
        grid-template-rows: max-content max-content max-content;
        grid-template-areas:
            "title video"
            "article video"
            "button video";
        justify-content: space-between;
        justify-items: space-between;
        align-content: space-between;
        align-items: center;
        gap: 0 87px;
    }

    @media only screen and (min-width: $lg) {
        padding: 48px;
        display: grid;
        grid-template-columns: auto max-content;
        grid-template-rows: max-content max-content max-content;
        grid-template-areas:
            "title video"
            "article video"
            "button video";
        justify-content: space-between;
        justify-items: space-between;
        align-content: space-between;
        align-items: center;
        gap: 0 77px;
    }
}

.proposal__title {
    margin: 0;
    text-align: left;
    width: max-content;
    color: var(--light-greyscale-bg-light, #FFF);
    font-style: normal;
    font-weight: 500;
    grid-area: title;
    grid-column: 1;


    @media only screen and (max-width: $sm) {
        font-size: 20px;
        line-height: 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 24px;
        line-height: 32px;
        text-transform: uppercase;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 28px;
        line-height: 36px;
        text-transform: uppercase;
    }

    @media only screen and (min-width: $lg) {
        font-size: 40px;
        line-height: 48px;
        text-transform: uppercase;
    }
}

.proposal__subtitle {
    text-align: left;
    margin: 0;
    color: var(--light-greyscale-bg-light, #FFF);
    grid-area: article;
    grid-column: 1;

    @media only screen and (max-width: $sm) {
        @include sm-caption;
        width: 100%;
        margin-top: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-caption;
        width: 100%;
        margin-top: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include md-caption;
        margin-top: 20px;
    }

    @media only screen and (min-width: $lg) {
        @include xm-caption;
        margin-top: 24px;
    }
}

.proposal__button {
    background: var(--light-greyscale-bg-light, #FFF);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    border-radius: 32px;
    color: var(--light-greyscale-text-primary, #04091D);
    z-index: 3;
    grid-area: button;
    grid-column: 1;

    @media only screen and (max-width: $sm) {
        @include sm-button-text;
        @include sm-button-space;
        margin-top: 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-button-text;
        @include lg-button-space;
        margin-top: 28px;
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

.proposal__button::after {
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

.proposal__video {
    border-radius: 20px;
    grid-area: video;
    grid-column: 2;

    @media only screen and (max-width: $sm) {
        margin-top: 44px;
        width: 100%;
        height: auto;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        margin-top: 32px;
        width: 100%;
        height: auto;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 488px;
        height: auto;
    }

    @media only screen and (min-width: $lg) {
        width: 654px;
        height: auto;
    }

}
</style>
