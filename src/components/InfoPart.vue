<template>
    <div class="info">
        <h6 class="info__name"> <span class="info__name-span"></span> Company</h6>
        <h1 class="title">Creative <span class="title__span">Marketing <span class="title__img"><img src="../assets/Bitmap.png" alt=""></span> </span></h1>
        <h2 class="info__title"></h2>
        <h4 class="info__sub-title"></h4>
        <p class="info__context">The sky was cloudless and of a deep dark blue the spectacle before us was indeed sublime.</p>
        <button class="btn btn_color_white">Explore</button>

    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
.info {
    width: 40%;
    &__name {
        font-weight: bold;
        font-size: 16px;
        line-height: 32px;
        color: #F07566;
        text-transform: uppercase;
        display: flex;
        gap: 6px;
        align-items: center;

        &-span {
            width: 12px;
            height: 12px;
            background: #F07566;
            border-radius: 50%;
            display: block;
        }
    }
    .title {
        font-weight: bold;
        font-size: 72px;
        line-height: 80px;
        color: #333333;
        margin-top: 24px;
        margin-bottom: 50px;
        &__span {
            color: #4DB282;
            position: relative;
        }
        &__img {
            position: absolute;
            left: 0;
            top: 30px;
        }
    }
    &__context {
        font-size: 20px;
        line-height: 32px;
        color: #333333;
        margin-bottom: 34px;
    }
}

@media only screen and (max-width: 500px) {
    .info {
        width: 100%;
        .title {
            font-size: 56px;
            line-height: 64px;
        }
    }
}
</style>