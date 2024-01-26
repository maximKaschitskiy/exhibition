<template>
    <section class="conditions">
        <div class="conditions__content">
            <p class="conditions__title">
                Специальные условия на технику Haier
            </p>
            <p class="conditions__subtitle">Широкий ассортимент бытовой техники для дома на специальных условиях для
                партнеров сети
            </p>
            <div class="conditions__privileges">
                <div class="conditions__privileges-item">
                    <img src="../../assets/prevelegies-box.svg" class="conditions__privileges-icon">
                    <p class="conditions__privileges-title">
                        Свой склад
                        <br>в Москве
                    </p>
                </div>
                <div class="conditions__privileges-item">
                    <img src="../../assets/prevelegies-truck.svg" class="conditions__privileges-icon">
                    <p class="conditions__privileges-title">
                        Бесплатная доставка
                        <br>в 15 регионах
                    </p>
                </div>
                <div class="conditions__privileges-item">
                    <img src="../../assets/prevelegies-tool.svg" class="conditions__privileges-icon">
                    <p class="conditions__privileges-title">
                        5 лет официальной
                        <br>гарантии
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.conditions {
    box-sizing: border-box;

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

.conditions__content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    flex-shrink: 0;
    box-sizing: border-box;
    z-index: 1;
    position: relative;
    background: #04091D;
    overflow: hidden;
    border-radius: 32px;

    background-position: bottom 0 right 0;
    background-repeat: no-repeat;
    z-index: 3;

    @media only screen and (max-width: $xs) {
        padding: 32px 16px;
        background-size: auto 55%;
        background-position: bottom 0 right -135px;
        background-image: url('../../assets/washingmachine_long.png');
    }

    @media only screen and (min-width: $xs) and (max-width: $sm) {
        padding: 32px 16px;
        background-size: auto 65%;
        background-position: bottom 0 right -100px;
        background-image: url('../../assets/washingmachine_long.png');
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 44px 24px;
        background-size: auto 100%;
        background-image: url('../../assets/washingmachine_long.png');
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 60px 32px;
        background-size: auto 100%;
        background-image: url('../../assets/washingmachine_long.png');
    }

    @media only screen and (min-width: $lg) {
        padding: 88px 48px;
        background-size: auto 100%;
        background-image: url('../../assets/washingmachine_long.png');
    }
}

.conditions__cards-bar {
    position: absolute;
    z-index: 3;
    bottom: 0;
    transform: translate(0, 50%);
}

.conditions__title {
    color: var(--light-greyscale-bg-light, #FFF);
    margin: 0;
    text-align: left;
    font-weight: 500;
    font-style: normal;

    @media only screen and (max-width: $xs) {
        font-size: 22px;
        line-height: 28px;
        width: 100%;
    }

    @media only screen and (min-width: $xs) and (max-width: $sm) {
        font-size: 22px;
        line-height: 28px;
        width: 275px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 28px;
        line-height: 36px;
        text-transform: uppercase;
        width: 375px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 36px;
        line-height: 44px;
        text-transform: uppercase;
        width: 475px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 40px;
        line-height: 48px;
        text-transform: uppercase;
        width: 550px;
    }
}

.conditions__subtitle {
    text-align: left;
    margin: 0;
    color: var(--light-greyscale-bg-light, #FFF);
    font-style: normal;
    font-weight: 300;

    @media only screen and (max-width: $xs) {
        font-size: 14px;
        line-height: 20px;
        width: 100%;
        margin-top: 16px;
    }

    @media only screen and (min-width: $xs) and (max-width: $sm) {
        font-size: 14px;
        line-height: 20px;
        width: 264px;
        margin-top: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 14px;
        line-height: 20px;
        width: 354px;
        margin-top: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 16px;
        line-height: 24px;
        width: 395px;
        margin-top: 20px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 20px;
        line-height: 28px;
        width: 550px;
        margin-top: 20px;
    }
}

.conditions__privileges {
    display: flex;

    @media only screen and (max-width: $sm) {
        margin-top: 32px;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
        gap: 20px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        margin-top: 40px;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
        gap: 16px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        margin-top: 40px;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
        gap: 24px;
    }

    @media only screen and (min-width: $lg) {
        margin-top: 52px;
        flex-direction: row;
        justify-content: space-between;
        align-items: flex-start;
        gap: 32px;
    }
}

.conditions__privileges-item {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;

    @media only screen and (max-width: $sm) {
        gap: 10px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        gap: 10px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        gap: 10px;
    }

    @media only screen and (min-width: $lg) {
        gap: 12px;
    }
}

.conditions__privileges-icon {
    @media only screen and (max-width: $sm) {
        width: 24px;
        height: 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        width: 28px;
        height: 28px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 28px;
        height: 28px;
    }

    @media only screen and (min-width: $lg) {
        width: 32px;
        height: 32px;
    }
}

.conditions__privileges-title {
    text-align: left;
    margin: 0;
    margin-left: 5px;
    color: var(--light-greyscale-stroke, #E6E6E8);
    font-style: normal;
    font-weight: 400;

    @media only screen and (max-width: $sm) {
        font-size: 12px;
        line-height: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 12px;
        line-height: 16px;
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
</style>
