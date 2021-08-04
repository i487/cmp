<template>
    <div class="project">
        <div class="project__example">
            <img :src="img" alt="" class="project__example-img">
            <div class="project__number"> {{ number }} </div>
        </div>
        <h4 class="project__title"> {{ name }} </h4>
        <p class="project__text"> {{ text }} </p>
    </div>
</template>

<script>
export default {
    name: "Project",
    props: ["number", "img", "name", "text"]
}
</script>

<style lang="scss">
.project {
     max-width: 570px;
    &__example {
        background: #D8D8D8;
        border-radius: 8px;
        max-width: 570px;
        
        height: 384px;
        position: relative;
        &-img {
            border-radius: 8px;
            max-width: 570px;
            width: 100%;
            object-fit: cover;
            height: 384px;
        }
    }
    &__number {
        background: #4DB282;
        border-radius: 0px 24px 0px 8px;
        font-weight: bold;
        font-size: 40px;
        line-height: 48px;
        color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 96px;
        height: 96px;
        position: absolute;
        bottom: 0;
        left: 0;
    }
    &__title {
        font-weight: bold;
        font-size: 24px;
        line-height: 32px;
        text-align: center;
        color: #333333;
        margin-top: 25px;
        margin-bottom: 4px;
    }
    &__text {
        font-size: 16px;
        line-height: 32px;
        text-align: center;
        color: rgba(51, 51, 51, 0.496405);
    }
}
</style>