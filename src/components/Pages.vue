<script setup>
import { ref } from 'vue';
import img1 from '../assets/pages1.svg';
import img2 from '../assets/pages2.svg';
import img3 from '../assets/pages3.svg';
import img4 from '../assets/pages4.svg';
import PagesCard from './PagesCard.vue';

    const cards = ref ([
        {
            id: 1,
            image: img1,
            name: 'Landig one'
        },
        {
            id: 2,
            image: img2,
            name: 'Landig two'
        },
        {
            id: 3,
            image: img3,
            name: 'Landig three'
        },
        {
            id: 4,
            image: img4,
            name: 'Landig four'
        },
    ]);
</script>

<template>
<section class="pages" id="landing__section">
    <div class="container pages__container">
        <h3 class="pages__title">Landing pages</h3>
        <div class="pages__list">
            <PagesCard
                v-for="card in cards" :key="card.id"
                :image="card.image" :name="card.name"
            />
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
.pages {
    padding: 100px;

    &__title {
        font-size: 40px;
        font-weight: 700;
        line-height: 120%;
        margin-bottom: 25px;
        color: black;
    }

    &__list {
        display: flex;
        flex-wrap: wrap;
        gap: 17px;
    }
}
</style>
