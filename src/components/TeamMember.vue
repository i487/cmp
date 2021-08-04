<template>
    <div class="member">
        <img :src="img" alt="" class="member__img">
        <h4 class="member__name"> {{ name }} </h4>
        <p class="member__position"> {{ job }} </p>
    </div>
</template>

<script>
export default {
    name: "TeamMember",
    props: ["img", "name", "job"]
}
</script>

<style lang="scss">
.member {
    padding: 16px;
    background: #FFFFFF;
    border: 1px solid #E6EDF5;
    border-radius: 8px;
    text-align: left;
    margin: 0 15px;
    
    &__img {
        border-radius: 8px 8px 50px 8px;
        max-width: 330px;
        width: 100%;
        height: 370px;
        pointer-events: none;
    }
    &__name {
        font-weight: bold;
        font-size: 24px;
        line-height: 32px;
        color: #333333;
    }
    &__position {
        font-size: 16px;
        line-height: 32px;
        color: rgba(51, 51, 51, 0.496405);
    }
}
</style>