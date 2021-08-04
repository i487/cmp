<template>
    <div class="partners">
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (1).png" alt=""></router-link>
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (2).png" alt=""></router-link>
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (3).png" alt=""></router-link>
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (4).png" alt=""></router-link>
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (5).png" alt=""></router-link>
        <router-link class="partners__item" to="/"><img src="../assets/Bitmap (6).png" alt=""></router-link>
    </div>
</template>

<script>
export default {
    name: "Partners"
}
</script>

<style lang="scss">
.partners {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    align-items: center;
    padding-top: 60px;
    padding-bottom: 40px;
}
@media only screen and (max-width: 500px) {
    .partners {
        justify-content: center;
        gap: 30px;
    }
}
</style>