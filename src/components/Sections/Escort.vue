<template>
    <section class="escort">
        <div class="escort__content">
            <div class="escort__content-wrapper">
                <h6 class="escort__content-title">
                    Маркетинговое сопровождение
                </h6>
                <p class="escort__content-article">
                    На старте бизнеса Вам не придется думать о том как эффективно привлекать клиентов, тратить время на
                    создание рекламного контента и вникать в маркетинговые инструменты самому.
                    <br>
                    <br>
                    Haier - уже широко узнаваемый бренд, с наработанными и проверенными рекламными стратегиями. Вы получите
                    рекламные креативы для трансляции в социальных сетях, помощь в настройке контекстной и таргетированной
                    рекламных кампаний, инструменты для СМС рассылок клиентам для увеличения продаж и многое другое!
                </p>
                <div class="escort__content-benefits">
                    <div class="escort__benefits-viewport">
                        <p class="escort__content-benefit">Интегрированная телефония</p>
                        <p class="escort__content-benefit">Генерация договора</p>
                        <p class="escort__content-benefit">Переписка в мессенджерах</p>
                        <p class="escort__content-benefit">Уникальная работа с заявками</p>
                        <p class="escort__content-benefit">Контроль курьеров и сборщиков</p>
                        <p class="escort__content-benefit">Онлайн оплата по договору</p>
                    </div>
                </div>
            </div>
            <div class="escort__content-wrapper escort__content-flare_right escort__content-wrapper_screen">
                <img class="escort__content-screen" src="../../assets/escort_1.png">
                <p class="escort__content-caption">
                    <span class="escort__content-accent">500 000</span>
                    <br>
                    посетителей сайта увидят ваши контакты
                </p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.escort {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: max-content;
    box-sizing: border-box;
    z-index: 0;
    overflow: visible;
    border-radius: 32px;
    padding: 0 12px;
}

.escort__content-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 24px;
    flex-direction: column;
    height: max-content;
    position: relative;

    @media only screen and (max-width: $sm) {
        gap: 20px;
        width: 100%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        gap: 20px;
        width: 100%;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        gap: 24px;
    }

    @media only screen and (min-width: $lg) {
        gap: 32px;
    }
}

.escort__content {

    justify-content: space-evenly;
    align-items: center;
    width: 100%;

    @media only screen and (max-width: $sm) {
        display: flex;
        flex-direction: column;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto;
        gap: 100px 52px;
        justify-items: center;
        align-content: space-evenly;
    }
}

.escort__title {
    color: var(--accent-2-primary, #001233);
    text-align: center;
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

.escort__content-title {
    margin: 0;
    text-align: left;
    color: var(--accent-2-primary, #001233);
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 16px;
        line-height: 22px;
        align-self: flex-start;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 16px;
        line-height: 24px;
        align-self: flex-start;
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

.escort__content-article {
    margin: 0;
    text-align: left;
    color: var(--light-greyscale-text-secondary, #4F5361);

    @media only screen and (max-width: $sm) {
        @include sm-caption;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include sm-caption;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include md-caption;
    }

    @media only screen and (min-width: $lg) {
        @include xm-caption;
    }
}

.escort__content-benefits {
    display: flex;
    margin: 0;
    width: 100%;

    @media only screen and (max-width: $sm) {
        justify-content: left;
        align-items: center;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 12px;
        overflow: hidden;
        overflow-x: auto;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        justify-content: left;
        align-items: center;
        flex-direction: row;
        flex-wrap: wrap;
        gap: 12px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {}
}

.escort__benefits-viewport {
    display: flex;
    flex-direction: row;


    @media only screen and (max-width: $sm) {
        width: max-content;
        gap: 8px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        width: 100%;
        flex-wrap: wrap;
        gap: 8px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 100%;
        flex-wrap: wrap;
        gap: 8px;
    }

    @media only screen and (min-width: $lg) {
        width: 100%;
        flex-wrap: wrap;
        gap: 8px;
    }
}

.escort__content-benefit {
    color: var(--accent-2-primary, #001233);
    font-style: normal;
    font-weight: 500;
    line-height: 16px;
    border: 1px solid var(--light-greyscale-dividers, #C0C2C7);
    background: var(--light-greyscale-bg-light, #FFF);
    width: max-content;
    margin: 0;

    @media only screen and (max-width: $sm) {
        font-size: 14px;
        line-height: 16px;
        padding: 8px 12px;
        border-radius: 10px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 14px;
        line-height: 16px;
        padding: 8px 16px;
        border-radius: 12px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 14px;
        line-height: 16px;
        padding: 8px 16px;
        border-radius: 12px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 18px;
        line-height: 20px;
        padding: 12px 20px;
        border-radius: 16px;
    }
}

.escort__content-wrapper_screen {
    @media only screen and (max-width: $sm) {
        margin-top: 36px;
        gap: 25px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        margin-top: 40px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        margin-top: 40px;
    }

    @media only screen and (min-width: $lg) {
        margin: 0;
    }
}

.escort__content-caption {
    text-align: center;
    align-self: center;
    color: #1E1079;
    margin: 0;
    font-style: normal;
    font-weight: 600;

    @media only screen and (max-width: $sm) {
        font-size: 12px;
        line-height: 18px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 18px;
        line-height: 24px;
    }
}

.escort__content-accent {
    text-align: center;
    background-color: #1E1079;
    color: #1E1079;
    background: linear-gradient(180deg, #1E1079, #110b46);
    background-size: 100%;
    background-repeat: repeat;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-background-clip: text;
    -moz-text-fill-color: transparent;
    font-style: normal;
    font-weight: 900;

    @media only screen and (max-width: $sm) {
        font-size: 52px;
        line-height: 56px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 58px;
        line-height: 60px;

    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 58px;
        line-height: 60px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 88px;
        line-height: 90px;
    }
}

.escort__content-wrapper_screen {

    @media only screen and (max-width: $sm) {
        gap: 2px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        gap: 2px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        gap: 8px;
    }

    @media only screen and (min-width: $lg) {
        gap: 8px;

    }
}

.escort__content-screen {
    z-index: 2;

    @media only screen and (max-width: $sm) {
        width: 100%;
        height: auto;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {}
}
</style>
