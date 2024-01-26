<script setup lang="ts">
  import available from '../Blocks/available.vue';
  import unavailable from '../Blocks/unavailable.vue';
</script>

<template>
    <section class="plans">
        <h6 class="plans__title">Тарифные планы</h6>
        <div class="plans__viewport">
            <table class="plans__table">
                <thead class="">
                    <tr class="">
                        <th class="plans__specs_head">
                            Что входит
                        </th>
                        <th class="plans__plan-head">
                            <p class="plans__plan-head-content">
                                <span class="plans__plan-head_accent">
                                    Бренд секция
                                </span>
                            </p>
                        </th>
                        <th class="plans__plan-head">
                            <p class="plans__plan-head-content">
                                <span class="plans__plan-head_accent">
                                    Фирменный салон
                                </span>
                                <br>
                                &lt; 50 кв. м.
                            </p>
                        </th>
                        <th class="plans__plan-head">
                            <p class="plans__plan-head-content">
                                <span class="plans__plan-head_accent">
                                    Фирменный салон
                                </span>
                                <br>
                                50 - 100кв. м.
                            </p>
                        </th>
                        <th class="plans__plan-head">
                            <p class="plans__plan-head-content">
                                <span class="plans__plan-head_accent">Фирменный салон</span>
                                <br>
                                &gt; 100 кв. м.
                            </p>
                        </th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Стоимость выставочного образца</td>
                        <td class="plans__specs">150 000 ₽&nbsp;</td>
                        <td class="plans__specs">125 000 ₽&nbsp;</td>
                        <td class="plans__specs">Бесплатно</td>
                        <td class="plans__specs plans__plan-item-end">Бесплатно</td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Скидка на технику Haier</td>
                        <td class="plans__specs">2%</td>
                        <td class="plans__specs">3%</td>
                        <td class="plans__specs">4%</td>
                        <td class="plans__specs plans__plan-item-end">5%</td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Обучение персонала</td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">CRM-система</td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Кухонный конструктор</td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Маркетинговое сопровождение</td>
                        <td class="plans__plan-item-center">
                            <unavailable></unavailable>
                        </td>
                        <td class="plans__plan-item-center">
                            <unavailable></unavailable>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Колл-центр</td>
                        <td class="plans__plan-item-center">
                            <unavailable></unavailable>
                        </td>
                        <td class="plans__plan-item-center">
                            <unavailable></unavailable>
                        </td>
                        <td class="plans__plan-item-center">
                            <unavailable></unavailable>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Склад в Москве</td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                    <tr class="plans__row">
                        <td class="plans__specs plans__plan-item-start">Обучение персонала</td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-center">
                            <available></available>
                        </td>
                        <td class="plans__plan-item-end">
                            <available></available>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>
</template>

<style scoped lang="scss">
.plans {
    display: flex;
    flex-direction: column;
    box-sizing: border-box;
    border-radius: 24px;
    background: var(--light-greyscale-bg-light, #FFF);

    @media only screen and (max-width: $sm) {
        align-items: flex-start;
        justify-content: center;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        align-items: center;
        justify-content: center;
        border: 1px solid var(--light-greyscale-stroke, #E6E6E8);
        padding: 32px 24px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        align-items: center;
        justify-content: center;
        border: 1px solid var(--light-greyscale-stroke, #E6E6E8);
        padding: 32px;
    }

    @media only screen and (min-width: $lg) {
        align-items: center;
        justify-content: center;
        border: 1px solid var(--light-greyscale-stroke, #E6E6E8);
        padding: 48px;
    }
}

.plans__viewport {
    width: 100%;

    @media only screen and (max-width: $sm) {
        overflow-x: scroll;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    @media only screen and (min-width: $lg) {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
}

.plans__viewport::-webkit-scrollbar {
    width: 4px;
    border-radius: 4px;
}

.plans__viewport::-webkit-scrollbar-track {
    width: 4px;
    background: var(--light-greyscale-bg-dark, #F6F7F9);
    border-radius: 4px;
}

.plans__viewport::-webkit-scrollbar-thumb {
    width: 4px;
    background: var(--light-greyscale-text-tertiary, #9B9DA5);
    border-radius: 4px;
}

.plans__viewport::-webkit-scrollbar-thumb:hover {
    background: #555;
}

.plans__row {
    text-align: center;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: 24px;
}

.plans__table {
    table-layout: auto;
    border-collapse: collapse;
    border-spacing: 10px;
    text-align: left;

    @media only screen and (max-width: $sm) {
        width: max-content;

    }

    @media only screen and (min-width: $sm) and (max-width: $md) {}

    @media only screen and (min-width: $md) and (max-width: $lg) {}

    @media only screen and (min-width: $lg) {
        width: 100%;

    }
}

.plans__plan-head {
    text-align: center;
    color: var(--accent-2-primary, #001233);
    position: relative;
    z-index: 3;
    width: max-content;

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
        @include xm-caption;
    }
}

.plans__plan-head::after {
    content: '';
    border-radius: 24px 24px 0px 0px;
    background: var(--light-greyscale-bg-dark, #F6F7F9);
    position: absolute;
    display: block;
    box-sizing: border-box;
    width: calc(100% - 10px);
    padding: 0 10px 0 10px;
    height: 100%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 0;
}

.plans__plan-head-content {
    z-index: 3;
    position: relative;

    @media only screen and (max-width: $sm) {
        width: max-content;
        padding: 0 24px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        padding: 0 24px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        padding: 0 12px;
    }

    @media only screen and (min-width: $lg) {
        padding: 0 24px;
    }
}

.plans__plan-head_accent {
    @media only screen and (max-width: $sm) {
        font-weight: 700;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-weight: 700;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-weight: 700;
    }

    @media only screen and (min-width: $lg) {
        font-weight: 500;
    }
}

.plans__specs_head {
    text-align: left;
    color: var(--accent-2-primary, #001233);
    font-style: normal;
    font-weight: 700;
    padding: 0 0 0 24px;

    @media only screen and (max-width: $sm) {
        font-size: 14px;
        line-height: 20px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 16px;
        line-height: 24px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 16px;
        line-height: 24px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 24px;
        line-height: 32px;
    }
}


.plans__title {
    color: var(--accent-2-primary, #001233);
    font-style: normal;
    font-weight: 500;
    margin: 0;
    text-align: center;
    caption-side: top;
    align-self: center;

    @media only screen and (max-width: $sm) {
        font-size: 22px;
        line-height: 28px;
        margin-bottom: 32px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        font-size: 24px;
        line-height: 32px;
        margin-bottom: 32px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        font-size: 28px;
        line-height: 36px;
        margin-bottom: 32px;
    }

    @media only screen and (min-width: $lg) {
        font-size: 40px;
        line-height: 48px;
        margin-bottom: 52px;
    }
}

.plans__plan-item-start {
    padding: 12px 0 12px 24px;
    border-radius: 8px 0 0 8px;
    text-align: left;
}

.plans__plan-item-end {
    padding: 12px 0 12px 0;
    border-radius: 0 8px 8px 0;
}

.plans__row {
    text-align: center;
    @include md-caption;
}

.plans__specs {
    color: var(--accent-2-primary, #001233);

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
        @include xm-caption;
    }
}

.plans__row:nth-child(even) {
    background-color: #f2f2f2;
}
</style>
