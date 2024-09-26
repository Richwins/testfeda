<script setup>

import HowComponent from '../HowComponent.vue'

import SessionComponent from '../SessionComponent.vue';

defineProps({
    menu_list: {
        type: String,
        required: true
    }
})
</script>

<template>
    <SessionComponent>
        <template #session-title>
            How it works
        </template>
        <template #session-subtitle>
            What We Serve
        </template>
        <template #session-description>
            Product Quality Is Our Priority, And Always Guarantees <br> Halal And Safety Until It Is In Your Hands.
        </template>
             <template #session-body>
              <div class="row">
                        <div class="col-lg-4">
                            <HowComponent title="Easy To Order " description="You only order through the app" img="/img/order 1.svg"></HowComponent>
                      

                        </div>
                        <div class="col-lg-4">
       <HowComponent title="Fastest Delivery " description="Delivery will be on time" img="/img/delivery 1.svg"></HowComponent>

                        </div>
                        <div class="col-lg-4">
                             <HowComponent title="Best Quality " description="The best quality of food for you" img="/img/courier 1.svg"></HowComponent>
                        </div>
                        </div>       
             </template>

    </SessionComponent>
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
