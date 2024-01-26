<template>
    <section class="benefit">
        <h5 class="benefit__title">Открывая салон под брендом Haier KitchenLab, вы получаете:</h5>
        <div class="benefit__item">
            <div class="benefit__item-wrapper">
                <p class="benefit__item-num">
                    /01
                </p>
                <p class="benefit__item-title">
                    Выставочные образцы в студию бесплатно
                </p>
                <p class="benefit__item-subtitle">
                    Мы берем на себя часть рисков открытия салона и предоставляем Выставочные образцы в студию бесплатно
                </p>
            </div>
        </div>
        <div class="benefit__item">
            <div class="benefit__item-wrapper">
                <p class="benefit__item-num">
                    /02
                </p>
                <p class="benefit__item-title">
                    Готовая бизнес-модель
                </p>
                <p class="benefit__item-subtitle">
                    Мебельного предприятия по продаже и сервисному обслуживанию со сроком окупаемости от 3х месяцев
                </p>
            </div>
        </div>
        <div class="benefit__item">
            <div class="benefit__item-wrapper">
                <p class="benefit__item-num">
                    /03
                </p>
                <p class="benefit__item-title">
                    Проверенные
                    <br>поставщики
                </p>
                <p class="benefit__item-subtitle">
                    Изделий из камня, аксессуаров фурнитуры и многого другого
                </p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.benefit {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: max-content;
    box-sizing: border-box;
    overflow: visible;

    @media only screen and (max-width: $sm) {
        padding: 12px;
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

.benefit__item {
    flex-direction: row;
    display: flex;
    align-items: center;
    justify-content: center;
    flex: 1;
    width: 100%;
    overflow: visible;
    position: relative;
    box-sizing: border-box;

    @media only screen and (max-width: $sm) {
        padding: 0 8px;
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

.benefit__item-wrapper {
    display: flex;
    box-sizing: border-box;
    justify-content: space-between;
    align-items: center;
    width: 100%;

    @media only screen and (max-width: $sm) {
        flex-direction: column;
        align-items: flex-start;
        padding: 20px 0;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        flex-direction: row;
        padding: 24px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        flex-direction: row;
        padding: 32px;
    }

    @media only screen and (min-width: $lg) {
        padding: 36px 48px;
    }

}

.benefit__title {
    text-align: center;
    margin: 0;
    color: var(--accent-2-primary, #001233);

    @media only screen and (max-width: $sm) {
        @include md-caption;
        margin-bottom: 28px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        @include lg-caption;
        margin-bottom: 44px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        @include xl-caption;
        margin-bottom: 44px;
    }

    @media only screen and (min-width: $lg) {
        @include xxl-caption;
        margin-bottom: 60px;
    }
}

.benefit__item-num {
    color: var(--accent-2-primary, #001233);
    margin: 0;
    font-style: normal;
    font-weight: 500;

    @media only screen and (max-width: $sm) {
        font-size: 20px;
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

.benefit__item-title {
    text-align: left;
    margin: 0;
    color: var(--accent-2-primary, #001233);

    @media only screen and (max-width: $sm) {
        font-size: 16px;
        font-style: normal;
        font-weight: 600;
        line-height: 22px;
        margin-top: 16px;
        width: 100%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 18px;
        font-style: normal;
        font-weight: 700;
        line-height: 26px;
        width: 214px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 28px;
        font-style: normal;
        font-weight: 700;
        line-height: 36px;
        width: 334px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 28px;
        font-style: normal;
        font-weight: 700;
        line-height: 36px;
        width: 334px;
    }
}

.benefit__item-subtitle {
    text-align: left;
    margin: 0;
    color: var(--light-greyscale-text-secondary, #4F5361);

    @media only screen and (max-width: $sm) {
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 20px;
        margin-top: 12px;
        width: 100%;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 20px;
        width: 291px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 16px;
        font-style: normal;
        font-weight: 400;
        line-height: 24px;
        width: 397px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 16px;
        font-style: normal;
        font-weight: 400;
        line-height: 24px;
        width: 397px;
    }
}

.benefit__item::after {
        content: '';
        width: 100%;
        height: 1px;
        background: var(--light-greyscale-stroke, #E6E6E8);
        position: absolute;
        left: 0;
        bottom: 0;
    }
</style>
