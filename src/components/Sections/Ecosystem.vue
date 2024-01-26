<template>
    <section class="ecosystem">
        <h5 class="ecosystem__title">
            Цифровая экосистема увеличивающая
            <br>продуктивность бизнеса до 10 раз!
        </h5>
        <div class="ecosystem__content">
            <div class="ecosystem__content-wrapper content__text-1">
                <h6 class="ecosystem__content-title">
                    CRM система заточенная под мебельный бизнес
                </h6>
                <p class="ecosystem__content-article">
                    Наш собственный продукт, созданный для работы с бизнес-процессами именно в мебельном бизнесе.
                    Незаменимый
                    помощник на всех этапах сделки от звонка до отзыва клиента о кухне. Вы сможете создавать уникальные
                    финансовые отчеты и контролировать показатели каждого сотрудника, а также видеть в прямом эфире где
                    находятся курьеры и сборщики.
                </p>
                <div class="ecosystem__content-benefits">
                    <div class="ecosystem__benefits-viewport">
                        <p class="ecosystem__content-benefit">Интегрированная телефония</p>
                        <p class="ecosystem__content-benefit">Генерация договора</p>
                        <p class="ecosystem__content-benefit">Переписка в мессенджерах</p>
                        <p class="ecosystem__content-benefit">Уникальная работа с заявками</p>
                        <p class="ecosystem__content-benefit">Контроль курьеров и сборщиков</p>
                        <p class="ecosystem__content-benefit">Онлайн оплата по договору</p>
                    </div>
                </div>
            </div>
            <div class="ecosystem__content-wrapper ecosystem__content-flare_right content__img-1">
                <img class="ecosystem__content-screen" src="../../assets/ecosystem_1.png">
            </div>
            <div class="ecosystem__content-wrapper content__text-2">
                <h6 class="ecosystem__content-title">
                    Легкий и функциональный кухонный конструктор
                </h6>
                <p class="ecosystem__content-article">
                    Простой в обучении конструктор для проектирования и дизайна кухни. Конструктор интегрирован с CRM, что
                    позволяет с легкостью отправлять проекты клиентам. Расчёт стоимости и проектная декларация генерируются
                    автоматически, позволяя дизайнерам полностью сосредоточиться на кухне. Обучение персонала берём на себя.
                </p>
                <div class="ecosystem__content-benefits">
                    <div class="ecosystem__benefits-viewport">
                        <p class="ecosystem__content-benefit">Простой в обучении</p>
                        <p class="ecosystem__content-benefit">Легкое 3D моделирование</p>
                        <p class="ecosystem__content-benefit">Клиент получает красивые рендеры</p>
                        <p class="ecosystem__content-benefit">Автоматический расчет стоимости</p>
                    </div>
                </div>
            </div>
            <div class="ecosystem__content-wrapper ecosystem__content-flare_left content__img-2">
                <img class="ecosystem__content-screen" src="../../assets/ecosystem_2.png">
            </div>
        </div>
        <!-- <div class="ecosystem__bg"></div> -->
    </section>
</template>

<style scoped lang="scss">
.ecosystem {
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

.ecosystem__content-wrapper {
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

.ecosystem__content {

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
        margin-top: 100px;
        justify-items: center;
        align-content: space-evenly;
    }
}

.content__text-1 {
    order: 1;

    @media only screen and (max-width: $sm) {
        margin-top: 32px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        margin-top: 48px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
       margin-top: 48px;
    }

    @media only screen and (min-width: $lg) {
        margin: 0;
    }
}

.content__text-2 {
    order: 3;

    @media only screen and (max-width: $sm) {
        margin-top: 64px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        margin-top: 84px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
       margin-top: 84px;
    }

    @media only screen and (min-width: $lg) {
        margin: 0;
    }
}

.content__img-1 {
    order: 2;

    @media only screen and (max-width: $sm) {
        margin-top: 54px;
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

.content__img-2 {
    order: 4;

    @media only screen and (max-width: $sm) {
        margin-top: 36px;
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

.ecosystem__title {
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

.ecosystem__content-title {
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

.ecosystem__content-screen {
    z-index: 2;

    @media only screen and (max-width: $sm) {
        width: 100%;
        height: auto;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {}
}

.ecosystem__content-article {
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

.ecosystem__content-benefits {
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

    @media only screen and (min-width: $md) and (max-width: $lg) {

    }

    @media only screen and (min-width: $lg) {

    }
}

.ecosystem__benefits-viewport {
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

.ecosystem__content-benefit {
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
</style>
