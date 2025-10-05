<script setup>

</script>

<template>
<section class="hero">
    <div class="container hero__container">
        <div class="main__info">
            <h1 class="main__info--title">Blanko template</h1>
            <p class="main__info--paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Odio mauris porttitor amet volutpat.</p>
            <div class="main__info--btn">
                <button class="main__info--btn__black">Purchase template</button>
                <button class="main__info--btn__white">Other templates</button>
            </div>
        </div>
        <img src="../assets/hero.svg" alt="">
    </div>
</section>
</template>

<style scoped lang="scss">
.hero {
    background-color: #FF7143;

    &__container {
        display: flex;
        align-items: center;
        gap: 231px;
        justify-content: space-between;
    }
}

.main__info {
    display: block;
    max-width: 600px;
    text-align: center;
    align-items: center;
    justify-content: center;

    &--title {
        color: black;
        font-size: 72px;
        font-weight: bold;
    }

    &--paragraph {
        color: black;
        padding: 27px 0px 22px 0px;
        font-size: 18px;
        line-height: 27px;
    }

    &--btn {
        display: flex;
        gap: 6px;
        justify-content: center;

        &__black {
            color: white;
            background: black;
            font-size: 18px;
            padding: 20px 32px;
            border-radius: 6px;
            border-color: black;
        }

        &__white {
            color: black;
            background: white;
            font-size: 18px;
            padding: 20px 32px;
            border-radius: 6px;
            border-color: white;
        }
    }
}
</style>
