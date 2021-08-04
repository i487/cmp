<template>
    <header class="header">
        <div class="container header__container">
            <div class="header__item">
                <router-link class="header__logo" to="/">CMP</router-link>
                <nav class="nav" :class="showing ? 'nav-show' : '' " >
                    <button class="close-btn" @click="show()">+</button>
                    <router-link class="nav__item" to="/about">About</router-link>
                    <router-link class="nav__item" to="/about">Portfolio</router-link>
                    <router-link class="nav__item" to="/about">Service</router-link>
                    <router-link class="nav__item" to="/about">Blog</router-link>
                    <router-link class="nav__item" to="/about">Contact</router-link>
                </nav>
            </div>
            <button class="btn">Contact</button>
            <div class="burger" @click="show()">
                <div class="burger__items">
                    <div class="burger__item"></div>
                    <div class="burger__item"></div>
                    <div class="burger__item"></div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data () {
        return {
            showing: false
        }
    },
    methods: {
        show() {
            this.showing = !this.showing
            console.log('working')
        }
    },
    watch:{
        show(){
            if (this.show){
                document.body.style.overflow = "hidden"
            } else {
                document.body.style.overflow = "scroll"
            }
        }
    }
}
</script>

<style lang="scss">
.header {
    padding: 16px 0; 
    &__container {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    &__item {
        display: flex;
        align-items: center;
        gap: 42px;
    }
    &__logo {
        font-weight: bold;
        font-size: 40px;
        line-height: 48px;
        color: #333333;
        text-decoration: none;
    }
    .nav {
        display: flex;
        align-items: center;
        gap: 40px;
        &__item {
            font-weight: normal;
            font-size: 16px;
            line-height: 32px;
            color: #333333;
            transition: 0.3s;
            &:hover {
                color: #745353
            }
        }
        .close-btn {
            background: white;
            padding: 10px;
            font-size: 26px;
            padding: 6px 14px;
            border-radius: 50%;
            font-weight: 700;
            transform: rotate(45deg);
            color: gray;
            border: 1px solid gray;
            display: none;


        }
    }
    .burger {
        display: none;
        width: 48px;
        height: 48px;
        background: #F07566;
        border-radius: 50%;
        text-align: center;
        &__items {
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            gap: 4px;
        }
        &__item {
            width: 28px;
            height: 3px;
            background: white;
        }
        
    }

}

@media only screen and (max-width: 450px) {
    .header {
        // position: fixed;
        // top: 0;
        // left: 0;
        width: 100%;
        background: gainsboro;
        .btn {
            display: none;
        }
        .burger {
            display: block;
        }
        // .nav {
        //     display: none;
        // }
        .nav {
            width: 100%;
            height: 100vh;
            background: palegreen;
            position: absolute;
            top: 0;
            left: -100%;
            flex-direction: column;
            padding-bottom: 20px;
            transition: 0.3s;
            .close-btn {
                display: block;
                margin-top: 10px;
            }
        }
        .nav-show {
            transition: 0.3s;
            left: 0;
        }
    }
}
</style>