<template>
    <section class="intro">
        <Info-part />
        <div class="intro__item">
            <img src="../assets/intro.png" alt="" class="intro__img">
        </div>
    </section>
</template>

<script>
import InfoPart from './InfoPart.vue'
export default {
  components: { InfoPart },
    name: "IntroSection"
}
</script>

<style lang="scss">
.intro {
    padding: 50px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    &__img {
        max-width: 420px;
        width: 100%;
    }
}
@media only screen and (max-width: 500px) {
    .intro {
        flex-direction: column-reverse;
        
    }
}
</style>