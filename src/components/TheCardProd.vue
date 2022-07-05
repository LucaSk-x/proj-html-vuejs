<template>
    <div class="h-100">
        <div class="card h-100 d-flex flex-column justify-content-between">
            <div class="img-contain">
                <img class="w-100" :src="img" alt="">
            </div>
            <div class="descript d-flex flex-column p-2">
                <div class="text-secondary">{{type}}</div>
                <div>{{title}}</div>
            </div>
            <div class="line m-2"></div>
            <div class="info d-flex justify-content-between  p-2">
                <div class="rating">
                    <span v-for="i in 5" :key="i">
                        <template v-if="i <= rating">
                            <img src="../../public/img/starfull.svg" alt="">
                        </template>
                        <template v-else>
                            <img src="../../public/img/staremptyl.svg" alt="">
                        </template>
                    </span>
                </div>
                <div>
                    <div class="text-secondary text-decoration-line-through">{{discountPrice}}</div>
                    <div class="text-end">{{price}}</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        img: String,
        type: String,
        title: String,
        rating: String,
        discountPrice: String,
        price: String,
    },
}
</script>

<style lang="scss">
    .line {
        border-top: 1px solid rgb(225, 225, 225);
    }
</style>