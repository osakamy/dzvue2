<script setup>

</script>

<template>
<section class="hero" id="hero__section">
    <div class="container hero__container">
        <div class="main__info">
            <h1 class="main__info--title">Blanko template</h1>
            <p class="main__info--paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Odio mauris porttitor amet volutpat.</p>
            <div class="main__info--btn">
                <button class="main__info--btn__black">Purchase template</button>
                <button class="main__info--btn__white">Other templates</button>
            </div>
        </div>
        <img class="hero__img" src="../assets/hero.svg" alt="">
    </div>
</section>
</template>

<style scoped lang="scss">
.hero {
    background-color: #FF7143;

    @media (max-width: 979px) {
            padding: 80px 0;
        }

    @media (max-width: 767px) {
        padding: 40px 0;
    }

    &__container {
        display: flex;
        align-items: center;
        gap: 231px;
        justify-content: space-between;

        @media (max-width: 1200px) {
            justify-content: space-around;
        }
    }
}

.main__info {
    display: block;
    max-width: 600px;
    text-align: center;
    align-items: center;
    justify-content: center;

    @media (max-width: 1200px) {
            max-width: 34rem;
    }

    @media (max-width: 767px) {
        max-width: 20rem;
    }

    &--title {
        color: black;
        font-size: 72px;
        font-weight: bold;

        @media (max-width: 1200px) {
            font-size: 3.5rem;
        }

        @media (max-width: 767px) {
            font-size: 2.5rem;
        }

        @media (max-width: 479px) {
            font-size: 1.5rem;
        }
    }

    &--paragraph {
        color: black;
        padding: 27px 0px 22px 0px;
        font-size: 18px;
        line-height: 27px;

        @media (max-width: 767px) {
            max-width: 18rem;
        }

        @media (max-width: 479px) {
            flex-direction: column;
            max-width: 12rem;
        }
    }

    &--btn {
        display: flex;
        gap: 6px;
        justify-content: center;

        @media (max-width: 1200px) {
            padding: 0.75rem 1.5rem;
        }

        @media (max-width: 767px) {
            font-size: 0.75rem;
            line-height: 100%;
            padding: 0.5rem 1rem;
        }

        @media (max-width: 479px) {
            padding: 1rem;
        }

        &__black {
            color: white;
            background: black;
            font-size: 18px;
            padding: 20px 32px;
            border-radius: 6px;
            border-color: black;

            &:hover {
                cursor: pointer;
            }
        }

        &__white {
            color: black;
            background: white;
            font-size: 18px;
            padding: 20px 32px;
            border-radius: 6px;
            border-color: white;

            &:hover {
                cursor: pointer;
            }
        }
    }
}

.hero__img {
    max-width: 26rem;
    width: 100%;

    @media (max-width: 1200px) {
        max-width: 15rem;
    }

    @media (max-width: 979px) {
        display: none;
    }
}
</style>
