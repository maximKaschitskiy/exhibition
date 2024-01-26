<script setup lang="ts">
</script>

<template>
    <section class="pluses-bar">
        <div class="pluses-bar__card">
            <div class="pluses-bar__head">
                <img class="pluses-bar__icon" src="../../assets/plus_icon.svg">
                <p class="pluses-bar__card-title">
                    Фильтрация входящих обращений собственным колл-центром
                </p>
            </div>
            <p class="pluses-bar__card-article">
                Колл-центр обрабатывает все входящие заявки и звонки и передает менеджерам уже теплые обращения, что
                снижает
                с них нагрузку и дает больше сосредоточиться на самом продукте и сервисе
            </p>
        </div>
        <div class="pluses-bar__card">
            <div class="pluses-bar__head">
                <img class="pluses-bar__icon" src="../../assets/plus_icon.svg">
                <p class="pluses-bar__card-title">
                    Помощь в обучении персонала
                </p>
            </div>
            <p class="pluses-bar__card-article">
                Налаженный процесс обучения и интеграции новых сотрудников в фирму сэкономит Ваше время и деньги,
                убережет
                от большинства ошибок, с которыми мы столкнулись за 20 лет работы компании
            </p>
        </div>
    </section>
</template>

<style scoped lang="scss">
.pluses-bar {
    box-sizing: border-box;

    @media only screen and (max-width: $sm) {
        padding: 0 12px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 12px;
        flex-direction: column-reverse;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 0 12px;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto;
        gap: 0 12px;
        justify-content: space-evenly;
        justify-items: center;
        align-content: space-evenly;
        align-items: center;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto;
        gap: 0 16px;
        justify-content: space-evenly;
        justify-items: center;
        align-content: space-evenly;
        align-items: center;
    }

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

.pluses-bar__card-title {
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

.pluses-bar__card {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
    border-radius: 32px;
    border: 1px solid var(--light-greyscale-stroke, #E6E6E8);
    background: var(--light-greyscale-bg-light, #FFF);
    width: 100%;
    height: 100%;
    box-sizing: border-box;

    @media only screen and (max-width: $sm) {
        padding: 20px 16px 24px 20px;
        gap: 16px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 24px 20px;
        gap: 12px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 40px 32px;
        gap: 24px;
    }

    @media only screen and (min-width: $lg) {
        padding: 40px 32px;
        gap: 24px;
    }
}

.pluses-bar__head {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    width: 100%;

    @media only screen and (max-width: $sm) {
        flex-direction: column;
        gap: 24px;
        justify-content: flex-start;
        align-items: flex-start;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        flex-direction: column;
        gap: 20px;
        justify-content: flex-start;
        align-items: flex-start;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        flex-direction: row;
        gap: 20px;
    }

    @media only screen and (min-width: $lg) {
        flex-direction: row;
        gap: 24px;
    }
}

.pluses-bar__icon {
    height: auto;

    @media only screen and (max-width: $sm) {
        width: 36px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {
        width: 44px;
    }
}

.pluses-bar__card-article {
    text-align: left;
    margin: 0;
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
</style>
