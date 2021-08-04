<template>
    <section class="articles">
        <div class="info info-center">
            <h6 class="info__name info__name-center"><span class="info__name-span"></span>Latest articles</h6>
            <h2 class="info__title">Check Our Insights</h2>
            <p class="info__context">See the face of Mars, anyhow, and that will be a rare experience seems to me that a view of the heavenly bodies through a fine telescope, as well as a tour round the world.</p>
        </div>
        <Article :article="article" :img="article.img" :title="article.title" />
        <button class="btn articles__btn">Browse all</button>
    </section>
</template>

<script>
import Article from './Article.vue'
export default {
  components: { Article },
    name: "Artciles",
    data () {
        return {
            article: [
                {
                    img: "https://picsum.photos/400/300",
                    title: "Above five feet square, was moving across",
                    text: "Truly it was a great journey, and in it I met with many, whom to know was to love."
                },
                {
                    img: "https://picsum.photos/400/300",
                    title: "Above five feet square, was moving across",
                    text: "Truly it was a great journey, and in it I met with many, whom to know was to love."
                },
                {
                    img: "https://picsum.photos/400/300",
                    title: "Above five feet square, was moving across",
                    text: "Truly it was a great journey, and in it I met with many, whom to know was to love."
                }
            ]
        }
    }
}
</script>

<style lang="scss">
.articles {
    margin-top: 100px;
    text-align: center;
    &__btn {
        margin-top: 60px;
    }
}
@media only screen and (max-width: 500px) {
    
}
</style>