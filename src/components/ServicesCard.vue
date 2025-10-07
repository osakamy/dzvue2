<script setup>
    const props = defineProps({
        image: String,
        title: String,
        description: String,
    });
</script>

<template>
    <div class="card">
        <img class="card__img" :src="props.image" alt="">
        <div class="card__content">
            <h3 class="card__content-title">{{ props.title }}</h3>
            <p class="card__content-description">{{ props.description }}</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .card {
        max-width: 416px;
        width: 100%;
        display: flex;
        gap: 24px;

        @media (max-width: 979px) {
            max-width: 560px;
        }

        @media (max-width: 767px) {
            max-width: 400px;
        }

        
        &__img {
            width: 100px;
            background: #FDE7DA;
            padding: 26px;
            
            @media (max-width: 1200px) {
                width: 84px;
            }

            @media (max-width: 979px) {
                max-width: 100px;
            }

            @media (max-width: 767px) {
                max-width: 80px;
            }
        }

        &__content {
            display: flex;
            flex-direction: column;
            gap: 13px;

            &-title {
                font-size: 24px;
                line-height: 133%;
                font-weight: 700;

                @media (max-width: 1200px) {
                    font-size: 20px;
                }

                @media (max-width: 979px) {
                    font-size: 20px;
                }

                @media (max-width: 767px) {
                    font-size: 16px;
                }
            }

            &-description {
                font-size: 16px;
                font-weight: 400;
                line-height: 150%;
            
                @media (max-width: 1200px) {
                    font-size: 12px;
                }

                @media (max-width: 979px) {
                    font-size: 16px;
                }

                @media (max-width: 767px) {
                    font-size: 12px;
                }
            }
        }
    }
</style>