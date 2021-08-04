<template>
    <section class="team">
        <div class="info info-center">
            <h6 class="info__name info__name-center"><span class="info__name-span"></span>Team</h6>
            <h2 class="info__title">Strong Members</h2>
            <p class="info__context">Formed a great hindrance to my speed, I resolved, contrary to my first intention, to make the being of a gigantic stature that is to say, about eight feet in height.</p>
        </div>
        <VueSlickCarousel v-bind="settings">
            <Team-member v-for="(item, index) in members" :key="index" :img="item.img" :name="item.name" :job="item.job" />
        </VueSlickCarousel>
        
    </section>
</template>
<script>
import TeamMember from './TeamMember.vue'
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
export default {
    components: { TeamMember, VueSlickCarousel },
    name: "Team",
    data () {
        return {
            members: [
                {
                    img: "https://picsum.photos/200/200",
                    name: "Ingo Schimpff",
                    job: "doctor"
                },
                {
                    img: "https://picsum.photos/200/200",
                    name: "Ingo Schimpff",
                    job: "doctor"
                },
                {
                    img: "https://picsum.photos/200/200",
                    name: "Ingo Schimpff",
                    job: "doctor"
                },
                {
                    img: "https://picsum.photos/200/200",
                    name: "Ingo Schimpff",
                    job: "doctor"
                },
            ],
            settings: {
                arrows: false,
                dots: true,
                slidesToShow: 3,
                responsive: [
                    {
                        breakpoint: 500,
                        settings: {
                            slidesToShow: 1,
                            slidesToScroll: 1,
                            infinite: true,
                            dots: true
                       }
                    }
                ]
            }
        }
    }
}
</script>

<style lang="scss">
.team {
    margin-top: 80px;
}
.slick-initialized .slick-slide {
    padding: 0 15px;
}
.slick-dots li button:before {
    color: #FFE4E1;
    opacity: 1;
}
.slick-dots li.slick-active button:before {
    transform: scale(2);
    color: #F07566;
}
.slick-current {
    box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
}
</style>