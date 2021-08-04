<template>
    <section class="contact">
        <div class="contact-box">
            <div class="contact-box__item">
                <h2 class="contact-box__title">Kickstart Your Next Project</h2>
                <button class="btn contact-box__btn">Contact us</button>
            </div>
            <div class="contact-box__item">
                <p class="contact-box__text">I shall see the face of Mars, anyhow, and that will be a rare experience. It seems to me that a view of the heavenly bodies through a fine telescope, as well as a tour round the world, should form a part of a liberal education.</p>
            </div>
            <img src="../assets/Bitmap (7).png" alt="" class="contact-box__img">
        </div>

        <form action="#" class="form">
            <h2 class="form__title">Company Newsletter</h2>
            <form class="form__inputs">
                <input type="email" class="form__input" placeholder="Your Email">
                <button class="btn form__btn">Subscribe</button>
            </form>
        </form>
    </section>
</template>

<script>
export default {
    name: "Contact",
}
</script>

<style lang="scss">
.contact {
    margin-top: 100px;
    .contact-box {
        background: #F07566;
        border-radius: 8px;
        padding: 80px 100px;
        display: flex;
        gap: 240px;
        position: relative;
        margin-bottom: 50px;
        &__img {
            position: absolute;
            bottom: -40px;
            right: 32%;
        }
        &__item {
            flex-basis: 50%;
        }
        &__title {
            font-weight: bold;
            font-size: 56px;
            line-height: 64px;
            color: #FFFFFF;
        }
        &__text {
            font-size: 16px;
            line-height: 32px;
            color: #FFFFFF;
        }
        &__btn {
            color: #333333;
            background: #FBD34B;
            margin-top: 30px;
        }
    }
    .form {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 50px;
        &__title {
            font-weight: bold;
            font-size: 40px;
            line-height: 48px;
            color: #333333;
        }
        &__inputs {
            display: flex;
            gap: 30px;
        }
        &__input {
            padding: 9px 16px;
            font-size: 16px;
            line-height: 32px;
            color: rgba(51, 51, 51, 0.496405);
            background: #FFFFFF;
            border: 1px solid #DADADA;
            border-radius: 6px;
        }
        &__btn {
            background: #F07566;
            color: #FFFFFF;
        }
    }
}
@media only screen and (max-width: 500px) {
    .contact {
        .contact-box {
            flex-direction: column;
            padding: 50px 60px;
            gap: 50px;
            &__item {
                flex-basis: 100%;
            }
            &__title {
                font-size: 40px;
                line-height: 48px;
            }
            &__text {
                padding-bottom: 100px;
            }
            &__img {
                right: 6%;
            }
        }
        .form {
            flex-direction: column;
            align-items: flex-start;

            &__inputs {
                margin-top: 36px;
                flex-direction: column;
                align-items: flex-start;
            }
        }
    }
}
</style>