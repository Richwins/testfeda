<script setup>

defineProps({
    btn_text: {
        type: String,
        required: true
    }
})</script>
<template>
    <button class="px-4 py-2 rounded-5 border-0">
        {{ btn_text }}
    </button>
</template>
<style scoped>
button {
    background-color: #FFCB45;
    font-size: 14px;
    font-weight: 600;
    color: #1D1D1D;
}
</style>