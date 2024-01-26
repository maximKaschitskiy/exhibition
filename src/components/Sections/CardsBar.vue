<template>
    <div class="cards-bar">
        <div class="cards-bar__card">
            <img class="cards-bar__icon" src="../../assets/card_pc.png">
            <div class="cards-bar__content">
                <p class="cards-bar__card-title">Бесплатная
                    <br>CRM система
                </p>
                <p class="cards-bar__card-subtitle">Подробнее</p>
            </div>
        </div>
        <div class="cards-bar__card">
            <img class="cards-bar__icon" src="../../assets/card_ai.png">
            <div class="cards-bar__content">
                <p class="cards-bar__card-title">ИИ, который делает
                    <br>проекты кухонь 24/7
                </p>
                <p class="cards-bar__card-subtitle">Подробнее</p>
            </div>
        </div>
        <div class="cards-bar__card">
            <img class="cards-bar__icon" src="../../assets/card_building.png">
            <div class="cards-bar__content">
                <p class="cards-bar__card-title">Бесплатный
                    <br>конструктор
                </p>
                <p class="cards-bar__card-subtitle">Подробнее</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.cards-bar {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    height: max-content;
    box-sizing: border-box;
    padding: 0 48px 0 48px;
    z-index: 3;
    transform: translate(0, -50%);
}

.cards-bar__card:first-child {
    margin-left: 0;
}

.cards-bar__card:last-child {
    margin-right: 0;
}

@media only screen and (max-width: 321px) {
    .cards-bar__card {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        flex-direction: row;
        padding: 32px 28px 32px 28px;
        margin-left: 8px;
        margin-right: 8px;
        flex: 1 auto;
        border-radius: 24px;
        border: 1px solid var(--light-greyscale-disabled-bg, #F2F3F4);
        background: var(--light-greyscale-white, #FFF);
        box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.04);
    }

    .cards-bar__card-title {
        color: var(--light-greyscale-bg-light, #FFF);
        margin: 0;
        text-align: left;
        font-size: 24px;
        font-style: normal;
        font-weight: 600;
        line-height: 32px;
        color: var(--accent-2-primary, #001233);
    }

    .cards-bar__card-subtitle {
        text-align: left;
        margin: 0;
        color: var(--light-greyscale-disabled-text, #6B6C72);
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 18px;
        margin-top: 12px;
    }

    .cards-bar__content {
        display: flex;
        flex-direction: column;
        margin-left: 8px;
    }

    .cards-bar__icon {
        width: 96px;
        height: auto;
        margin-right: 8px;
    }

}

@media only screen and (min-width: 297px) and (max-width: 740px) {
    .calculate {}

}

@media only screen and (min-width: 741px) and (max-width: 1320px) {
    .calculate {}

}

@media only screen and (min-width: 1321px) {
    .cards-bar__card {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        flex-direction: row;
        padding: 32px 28px 32px 28px;
        margin-left: 8px;
        margin-right: 8px;
        flex: 1 auto;
        border-radius: 24px;
        border: 1px solid var(--light-greyscale-disabled-bg, #F2F3F4);
        background: var(--light-greyscale-white, #FFF);
        box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.04);
    }

    .cards-bar__card-title {
        color: var(--light-greyscale-bg-light, #FFF);
        margin: 0;
        text-align: left;
        font-size: 24px;
        font-style: normal;
        font-weight: 600;
        line-height: 32px;
        color: var(--accent-2-primary, #001233);
    }

    .cards-bar__card-subtitle {
        text-align: left;
        margin: 0;
        color: var(--light-greyscale-disabled-text, #6B6C72);
        font-size: 14px;
        font-style: normal;
        font-weight: 400;
        line-height: 18px;
        margin-top: 12px;
    }

    .cards-bar__content {
        display: flex;
        flex-direction: column;
        margin-left: 8px;
    }

    .cards-bar__icon {
        width: 96px;
        height: auto;
        margin-right: 8px;
    }

}
</style>
