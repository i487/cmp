<template>
    <section class="strategy">
        <div class="container strategy__container">
            <div class="strategy__item">
                <img src="../assets/Group 5.png" alt="" class="strategy__img">
            </div>
            <div class="strategy__item">
                <h2 class="strategy__title">Strategy, technology and design</h2>
                <p class="strategy__text">Apparently we had reached a great height in the atmosphere, for the sky was a dead black.</p>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: "Strategy",
}
</script>

<style lang="scss">
.strategy {
    background: #F07566;
    margin-top: 180px;
    height: 400px;
    &__container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    &__item {
        flex-basis: 50%;
        position: relative;
        margin-top: 86px;
    }
    &__img {
        position: absolute;
        top: -245px;
    }
    &__title {
        font-weight: bold;
        font-size: 56px;
        line-height: 64px;
        color: #FFFFFF;
        margin-bottom: 26px;
    }
    &__text {
        font-size: 20px;
        line-height: 32px;
        color: #FFFFFF;
    }
}

@media only screen and (max-width: 500px) {
    .strategy {
        padding: 60px 0;
        height: 100%;
        &__img {
            position: initial;
        }
        &__title {
            font-size: 40px;
            line-height: 48px;
        }
        &__container {
            flex-direction: column;
        }
    }
}
</style>