<script setup>

defineProps({
    img: {
        type: String,
        required: true
    },
    title: {
        type: String,
        required: true
    },
    description: {
        type: String,
        required: true
    }

})
</script>

<template>
<div class="px-lg-4">
    <img :src="img" class="img-fluid">
    <h3>{{title}}</h3>
    <p>{{description}}</p>
</div>
</template>

<style scoped>
h3{
font-size: 28px;
font-weight: 600;
line-height: 35px;
text-align: center;
color:#1D1D1D;

}


</style>
