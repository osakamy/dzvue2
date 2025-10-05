<script setup>

</script>

<template>
<section class="services">
    <div class="container secvices__container">
        <div class="services__cards">
            <div class="services__card">
                <img src="../assets/speed.svg" alt="">
                <div class="services__card--info">
                    <h3 class="services__card--info__title">Speed</h3>
                    <p class="services__card--info__paragraph">Open a commercial-grade current account from anywhere</p>
                </div>
            </div>
            <div class="services__card">
                <img src="../assets/design.svg" alt="">
                <div class="services__card--info">
                    <h3 class="services__card--info__title">Design</h3>
                    <p class="services__card--info__paragraph">Open a commercial-grade current account from anywhere</p>
                </div>
            </div>
            <div class="services__card">
                <img src="../assets/modularity.svg" alt="">
                <div class="services__card--info">
                    <h3 class="services__card--info__title">Modularity</h3>
                    <p class="services__card--info__paragraph">Open a commercial-grade current account from anywhere</p>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
.services {
    padding: 85px 0px 85px 0px;

    &__container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    &__cards {
        display: flex;
    }

    &__card {
        display: flex;
        align-items: center;
        gap: 24px;

        &--info {
            color: black;

            &__title {
                font-weight: bold;
                font-size: 24px;
                padding-bottom: 13px;
            }
        }
    }
}
</style>
