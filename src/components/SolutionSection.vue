<template>
    <section class="solution">
        <div class="info">
            <h6 class="info__name"><span class="info__name-span"></span>Features</h6>
            <h2 class="info__title">Smart Complex Solutions</h2>
            <p class="info__context">Stars had ceased to twinkle the same illusion which lifts the horizon of the sea to the level of the spectator on a hillside, the sable cloud beneath was dished out.</p>
            <div class="info__box">
                <h3 class="info__box-title"> 
                    <span>
                        <svg width="24" height="23" viewBox="0 0 24 23" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path fill-rule="evenodd" clip-rule="evenodd" d="M8.332 7.62569L12 0L15.668 7.6267L24 8.78546L17.936 14.6569L19.416 22.999L12 19.0028L4.584 23L6.064 14.6579L0 8.78546L8.332 7.62569ZM14.335 9.47468L12 4.62096L9.665 9.47468L4.36 10.2133L8.221 13.9515L7.279 19.2617L12 16.7175L16.721 19.2607L15.779 13.9505L19.64 10.2123L14.335 9.47468Z" fill="#4DB282"/>
                        </svg>
                    </span> 
                    Modern Technology
                </h3>
                <p class="info__box-text">The sky was cloudless and of a deep dark blue the spectacle before us was indeed sublime.</p>
            </div>
        </div>
        <div class="solution__item">
            <img src="../assets/solut.png" alt="" class="solution__img">
        </div>
    </section>
</template>
<script>
export default {
    name: "SolutionSection"
}
</script>

<style lang="scss">
.solution {
    padding-top: 150px;
    display: flex;
    justify-content: space-between;

    &__img {
        max-width: 420px;
        width: 100%;
    }
    .info {
        &__box {
            background: #FFFFFF;
            box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
            border-radius: 8px;
            padding: 26px 32px;
            &-title {
                font-weight: bold;
                font-size: 24px;
                line-height: 32px;
                color: #333333;
                display: flex;
                align-items: center;
                gap: 10px;
            }
            &-text {
                font-size: 14px;
                line-height: 24px;
                color: rgba(51, 51, 51, 0.496405);
            }
        }
    }
}

@media only screen and (max-width: 500px) {
    .solution {
        flex-direction: column;
    }
    .info {
        margin-bottom: 70px;
        &__title {
            font-size: 40px;
            line-height: 48px;
        }
    }
}
</style>