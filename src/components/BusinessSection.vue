<template>
    <section class="business">
        <div class="business__image"><img src="../assets/Group2.png" alt="" class="business__img"></div>
        <div class="info">
            <h6 class="info__name"><span class="info__name-span"></span>About</h6>
            <h2 class="info__title">We Build PRO Business</h2>
            <h4 class="info__sub-title">Excited to work with customers</h4>
            <ul class="info__list">
                <li class="info__list-item"> 
                    <span><svg width="24" height="22" viewBox="0 0 24 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z" fill="#4DB282"/>
                        </svg>
                    </span>
                    The sky was cloudless and of a deep     
                </li>
                <li class="info__list-item">
                    <span><svg width="24" height="22" viewBox="0 0 24 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z" fill="#4DB282"/>
                        </svg>
                    </span>
                    Spectacle before us was indeed 
                </li>
                <li class="info__list-item">
                    <span><svg width="24" height="22" viewBox="0 0 24 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z" fill="#4DB282"/>
                        </svg>
                    </span>
                    Cloudless and of a deep dark 
                </li>
            </ul>
            <button class="btn btn_color_white">Explore</button>
        </div>
    </section>
</template>

<script>
export default {
    name: "BusinessSection"
}
</script>

<style lang="scss">
.business {
    display: flex;
    justify-content: space-between;
    // align-items: center;
    padding-bottom: 100px;
    &__img {
        max-width: 420px;
        width: 100%;
    }

}
.info {
    &__title {
        font-weight: bold;
        font-size: 56px;
        line-height: 64px;
        color: #333333;
        margin: 20px 0;
    }
    &__sub-title {
        font-weight: bold;
        font-size: 24px;
        line-height: 32px;
        color: #333333;
        margin-bottom: 34px;
    }
    &__list {
        margin-bottom: 30px;
        &-item {
            font-size: 16px;
            line-height: 32px;
            color: #333333;
        }
    }
}

@media only screen and (max-width: 500px) {
    .business {
        flex-direction: column;
    }
    .info {
        &__title {
            font-size: 40px;
            line-height: 48px;
        }
    }
}
</style>