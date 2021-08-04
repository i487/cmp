<template>
    <section class="portfolio">
        <div class="info info-center">
            <h6 class="info__name info__name-center"><span class="info__name-span"></span>Portfolio</h6>
            <h2 class="info__title">Company Cases</h2>
            <p class="info__context">Stars had ceased to twinkle the same illusion which lifts the horizon of the sea to the level of the spectator on a hillside, the sable cloud beneath was dished out.</p>
        </div>
        <div class="portfolio__projects">
            <Project  v-for="(item, index) in projects" :key="index" :number="item.number" :img="item.img" :name="item.name" :text="item.text" />
        </div>
        <button class="btn">Browse all</button>
    </section>
</template>

<script>
import Project from './Project.vue'
export default {
  components: { Project },
    name: "Portfolio",
    data () {
        return {
            projects: [
                {
                    number: "01",
                    img: 'https://picsum.photos/200/200',
                    name: "Face of Mars",
                    text: 'Will be a rare experience'
                },
                {
                    number: "02",
                    img: 'https://picsum.photos/201/200',
                    name: "Heavenly Bodies",
                    text: 'Tour round the world should form'
                },
                {
                    number: "03",
                    img: 'https://picsum.photos/200/201',
                    name: "Liberal Education",
                    text: 'Truly it was a great journey'
                },
                {
                    number: "04",
                    img: 'https://picsum.photos/202/200',
                    name: "Though the Gravity",
                    text: 'Daily classes he no longer collapsed'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
.portfolio {
    text-align: center;
    
    
    &__projects {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 50px 30px;
        padding-bottom: 60px;
    }
}
.info-center {
    text-align: center;
    width: 60%;
    margin: auto;
}
.info__name-center {
    justify-content: center;
}
@media only screen and (max-width: 500px) {
    .portfolio {
        &__projects {
            grid-template-columns: 1fr;
        }
    }
    .info-center {
        width: 100%;

    }
}
</style>