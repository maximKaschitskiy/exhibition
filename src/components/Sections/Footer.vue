<script setup lang="ts">
</script>

<template>
    <section class="footer">
        <img class="footer__bg-image" src="../../assets/pavilion.png">
        <div class="footer__content">
            <h2 class="footer__title">
                Мы на выставке
                <br>Мебель Экспо 2023
            </h2>
            <div class="footer__contact-wrapper">
                <p class="footer__caption">Стенд</p>
                <p class="footer__contact footer__contact_bold">FB020</p>
            </div>
            <div class="footer__contact-wrapper">
                <p class="footer__caption">Телефон</p>
                <p class="footer__contact">+7 (999) 999-99-99</p>
            </div>
            <div class="footer__contact-wrapper">
                <p class="footer__caption">Для предложений</p>
                <p class="footer__contact">b2b@haierkitchen.ru</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.footer {
    display: flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    z-index: 0;
    position: relative;
    background: #04091D;
    overflow: hidden;

    @media only screen and (max-width: $sm) {
        flex-direction: column-reverse;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        gap: 32px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        gap: 14px;
    }

    @media only screen and (min-width: $lg) {
        gap: 16px;
        flex-direction: row;
    }
}

.footer__content {
    width: 100%;
    z-index: 4;
    box-sizing: border-box;
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-direction: column;

    @media only screen and (max-width: $sm) {
        padding: 28px 12px;
        gap: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 40px 0 40px 0;
        gap: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 40px 0 40px 16px;
        gap: 20px;
    }

    @media only screen and (min-width: $lg) {
        padding: 48px 0 48px 33px;
        gap: 24px;
        width: max-content;
    }
}

.footer__bg-image {
    height: auto;
    margin-top: auto;

    @media only screen and (max-width: $sm) {
        width: 100%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        max-width: 566px;
        min-width: 500px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 663px;
    }

    @media only screen and (min-width: $lg) {
        width: 875px;
    }
}

.footer__contact-wrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
}

.footer__bg {
    width: 100%;
    height: 100%;
    z-index: 3;
}

.footer::after {
    content: '';
    display: block;
    z-index: 2;
    box-sizing: border-box;
    position: absolute;
    width: 294px;
    height: 287px;
    border-radius: 294px;
    background: #1F107C;
    filter: blur(110px);
    top: -60px;
    right: 0;

}

.footer__caption {
    text-align: left;
    color: var(--light-greyscale-text-tertiary, #9B9DA5);
    margin: 0;
    margin-bottom: 2px;
    font-weight: 400;
    font-style: normal;

    @media only screen and (max-width: $sm) {
        font-size: 12px;
        line-height: 18px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 12px;
        line-height: 14px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 16px;
        line-height: 24px;
    }
}

.footer__title {
    color: var(--light-greyscale-bg-light, #FFF);
    margin: 0;
    text-align: left;
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 20px;
        line-height: 24px;
        margin-bottom: 8px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 24px;
        line-height: 32px;
        margin-bottom: 8px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 28px;
        line-height: 36px;
        margin-bottom: 12px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 36px;
        line-height: 44px;
        margin-bottom: 12px;
    }
}

.footer__contact {
    text-align: left;
    color: var(--light-greyscale-bg-light, #FFF);
    margin: 0;
    margin-top: 2px;
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 16px;
        line-height: 24px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 20px;
        line-height: 28px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 24px;
        line-height: 32px;
    }
}

.footer__contact_bold {
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 16px;
        line-height: 22px;
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
</style>
