<script setup>
    import { ref } from 'vue';
    import OptionsCard from './ServicesCard.vue';
    import cardSpeed from '../assets/speed.svg';
    import cardDesign from '../assets/design.svg';
    import cardModularity from '../assets/modularity.svg';

    const cards = ref([
        {
            id: 1,
            image: cardSpeed,
            title: "Speed",
            description: "Open a commercial-grade current account from anywhere",
        },
        {
            id: 2,
            image: cardDesign,
            title: "Design",
            description: "Open a commercial-grade current account from anywhere",
        },
        {
            id: 3,
            image: cardModularity,
            title: "Modularity",
            description: "Open a commercial-grade current account from anywhere",
        },
    ]);
</script>

<template>
    <section class="services">
        <div class="container">
            <div class="services__cards">
                <OptionsCard
                    v-for="card in cards" :key="card.id"
                    :image="card.image" :title="card.title" :description="card.description"
                />
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    .services {
        padding: 80px 0;

        &__cards{
            display: flex;
            justify-content: space-between;
            gap: 16px;

            @media (max-width: 979px) {
                flex-direction: column;
                align-items: center;
            }
        }
    }
</style>