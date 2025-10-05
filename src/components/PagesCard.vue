<script setup>
    const props = defineProps ({
        image: String,
        name: String,
    });
</script>

<template>
    <div class="card">
        <img class="card__img" :src="props.image" alt="">
        <p class="card__name">{{ props.name }}</p>
    </div>
</template>

<style scoped lang="scss">
    .card {
        max-width: 414px;
        width: 100%;
        border-radius: 1px;

        &__img {
            width: 100%;
            background: black;
            padding: 40px 40px 0px 40px;
        }

        &__name {
            font-size: 20px;
            line-height: 28px;
            color: black;
            font-weight: 700;
            padding: 24px 0px 25px 32px;
        }
    }
</style>