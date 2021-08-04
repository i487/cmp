<template>
    <div>
        <article class="article">
            <img src="https://picsum.photos/600/400" alt="" class="article__img">
            <div class="article__context">
                <h2 class="article__title">What looked like a small patch of purple grass</h2>
                <p class="article__text">Truly it was a great journey, and in it I met with many, whom to know was to love.</p>
            </div>
        </article>
        <div class="article-wrapper">
            <div class="min-article" v-for="(item, index) in article" :key="index">
                <img :src="item.img" alt="" class="min-article__img">
                <router-link to="/"><h2 class="min-article__title"> {{ item.title }} </h2></router-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Article",
    props: ["article","img", "title"]
}
</script>

<style lang="scss">
.article {
    background: #FFFFFF;
    border: 1px solid #E6EDF5;
    border-radius: 8px;
    padding: 16px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 66px;
    &__img {
        border-radius: 8px 8px 50px 8px;
        max-width: 554px;
        width: 100%;
        height: 336px;
        object-fit: cover;
    }
    &__title {
        font-weight: bold;
        font-size: 40px;
        line-height: 48px;
        color: #333333;
        margin-bottom: 30px;
    }
    &__text {
        font-size: 20px;
        line-height: 32px;
        color: #333333;
    }

}
.article-wrapper {
    display: flex;
    gap: 30px;
    margin-top: 20px;
}
.min-article {
    background: #FFFFFF;
    border: 1px solid #E6EDF5;
    border-radius: 8px;
    padding: 16px;
    cursor: pointer;
    transition: 0.3s;
    &:hover {
        box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
    }
    &__img {
        max-width: 338px;
        width: 100%;
        height: 240px;
        border-radius: 8px 8px 50px 8px;
        margin-bottom: 25px;
    }
    &__title {
        font-weight: bold;
        font-size: 24px;
        line-height: 32px;
        color: #333333;
        text-align: center;
        padding: 0 15px;
    }
}
@media only screen and (max-width: 500px) {
    .article {
        flex-direction: column;
        text-align: left;
    }
    .article-wrapper {
        flex-direction: column;
    }
}
</style>