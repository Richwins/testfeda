<script setup>
import IconSearch from '../icons/IconSearch.vue';
import IconCart from '@/components/icons/IconCart.vue';
import ButtonComponent from '../ButtonComponent.vue';

defineProps({
    menu_list: {
        type: String,
        required: true
    }
})
</script>

<template>
    <header>
        <div class="header container py-2">
            <div class="row d-flex justify-content-between align-items-center">
                <div class="col-lg-3 text-center d-flex  align-items-center">
                    <img src="/img/logo.svg" alt="">
                </div>
                <div class="col-lg-6 d-none d-lg-flex  align-items-center">
                    <div class="menu-list col-12 p-0">
                        <ul class="d-flex align-items-center justify-content-between col-12 p-0 m-0">
                            <li class="menu-item active">Home</li>
                            <li class="menu-item">Menu</li>
                            <li class="menu-item">How it works</li>
                            <li class="menu-item">About</li>
                            <li class="menu-item">Contact</li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3 d-flex align-items-center justify-content-end">
                    <IconSearch class="mx-4" />
                    <IconCart class="mx-4" />
                    <ButtonComponent btn_text="Sign in" class="ml-4" />
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: #FFF9EA;

}

.menu-item {
    font-size: 19.8px;
    list-style: none;
    color: #1D1D1DB2;
    display: inline-flex;
    padding: 10px;
    font-weight: 500;
}

.menu-item.active {
    color: #1D1D1D;
}

.menu-item.active::after {
    height: 2px;
    background-color: #FFCB45;
    width: 100%
}
</style>
