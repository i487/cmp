<template>
    <section class="reviews">
        <div class="solution__item">
            <img src="../assets/Group 6.png" alt="" class="solution__img">
        </div>
        <div class="info">
            <h6 class="info__name"><span class="info__name-span"></span>Testimonials</h6>
            <h2 class="info__title">Reviews</h2>
            <div class="reviews__box">
                <img src="../assets/Shape.png" alt="" class="reviews__box-shape">
                <p class="reviews__box-text">"The sky was cloudless and of a deep dark blue the spectacle before us was indeed sublime sky was cloudless and of a deep dark."</p>
                <h3 class="reviews__box-title"> 
                    Jaroslav Brabec
                </h3>
                <p class="reviews__box-text">Microsoft</p>
                
            </div>
            <div class="arrows">
                <span class="arrows__item">
                    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="48" height="48" rx="24" fill="#F07566"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M16.3258 23.2196L25.4156 14.3195C25.6258 14.1135 25.9065 14 26.2057 14C26.5049 14 26.7856 14.1135 26.9958 14.3195L27.6652 14.9748C28.1008 15.4018 28.1008 16.0958 27.6652 16.5221L20.0323 23.9959L27.6737 31.4779C27.8839 31.6839 28 31.9586 28 32.2514C28 32.5446 27.8839 32.8192 27.6737 33.0254L27.0043 33.6805C26.7939 33.8865 26.5134 34 26.2142 34C25.9149 34 25.6343 33.8865 25.424 33.6805L16.3258 24.7723C16.1151 24.5656 15.9993 24.2897 16 23.9963C15.9993 23.7019 16.1151 23.4261 16.3258 23.2196Z" fill="white"/>
                    </svg>
                </span>
                <span class="arrows__item">
                    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="48" height="48" rx="24" fill="#F07566"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M31.6742 23.2196L22.5844 14.3195C22.3742 14.1135 22.0935 14 21.7943 14C21.4951 14 21.2144 14.1135 21.0042 14.3195L20.3348 14.9748C19.8992 15.4018 19.8992 16.0958 20.3348 16.5221L27.9677 23.9959L20.3263 31.4779C20.1161 31.6839 20 31.9586 20 32.2514C20 32.5446 20.1161 32.8192 20.3263 33.0254L20.9957 33.6805C21.2061 33.8865 21.4866 34 21.7858 34C22.0851 34 22.3657 33.8865 22.576 33.6805L31.6742 24.7723C31.8849 24.5656 32.0007 24.2897 32 23.9963C32.0007 23.7019 31.8849 23.4261 31.6742 23.2196Z" fill="white"/>
                    </svg>
                </span>
            </div>
        </div>
        
    </section>
</template>

<script>
export default {
    name: "reviews"
}
</script>

<style lang="scss">
.reviews {
    padding-top: 100px;
    display: flex;
    justify-content: space-between;

    &__box {
        background: #FFFFFF;
        box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
        border-radius: 8px;
        padding: 27px 32px;
        position: relative;
        &-shape {
            position: absolute;
            top: -4px;
            right: 25px;
        }
        &-text {
            font-size: 16px;
            line-height: 32px;
            color: rgba(51, 51, 51, 0.496405);
        }
        &-title {
            font-weight: bold;
            font-size: 24px;
            line-height: 32px;
            color: #333333;
            padding-top: 14px;
            padding-bottom: 6px;
        }
    }
    .arrows {
        margin-top: 48px;
        display: flex;
        align-items: center;
        gap: 6px;
    }
}
@media only screen and (max-width: 500px)  {
    .reviews {
        flex-direction: column;
    }
    .arrows {
        justify-content: center;
    }
}
</style>