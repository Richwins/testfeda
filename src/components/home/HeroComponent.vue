<script setup>

import ButtonComponent from '../ButtonComponent.vue';

defineProps({
    menu_list: {
        type: String,
        required: true
    }
})
</script>

<template>
    <div class="col-12 hero-session ">
        <div class="container">
            <div class="row d-flex align-items-center">
                <div class="col-lg-6 py-lg-5">
                    <h1>Be The Fastest In Delivery Your <span>Food</span> </h1>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit ut aliquam, purus sit amet
                    </p>
                    <ButtonComponent btn_text="Get started" />
                </div>
                <div class="col-lg-6 text-center pt-lg-5 pb-4 "><img src="/img/img-hero.png" alt=""></div>
            </div>

        </div>
    </div>


</template>

<style scoped>
.hero-session {
    background-color: #FFF9EA;
    background: url('/img/shapes.png');
    background-size: cover;
}

h1 {
    font-size: 48px;
    font-weight: 600;
    line-height: 60px;
    text-align: left;
}

h1 span {
    color: #FFCB45;
}

.hero-session p {
    font-size: 18px;
    font-weight: 400;
    line-height: 22.5px;
    text-align: left;
}
</style>
