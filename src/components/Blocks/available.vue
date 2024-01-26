<script setup lang="ts">
</script>

<template>
    <div class="available">
        <img class="available__icon" src="../../assets/available.svg">
    </div>
</template>

<style scoped lang="scss">
.available {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    border-radius: 8px;
    background: var(--light-system-successful, #00D615);
    margin: auto;

    @media only screen and (max-width: $sm) {
        width: 20px;
        height: 20px;
    }

    @media only screen and (min-width: $sm) and (max-width: $md) {
        width: 20px;
        height: 20px;
    }

    @media only screen and (min-width: $md) and (max-width: $lg) {
        width: 24px;
        height: 24px;
    }

    @media only screen and (min-width: $lg) {
        width: 24px;
        height: 24px;
    }
}

.available__icon {
    
}
</style>
