<template>
    <section class="col-12">
        <div class="whatweserve container ">
            <div class="row d-flex justify-content-center text-center">
                <div class="header-session">
                    <div class="session-title">
                        <slot name="session-title"></slot>
                    </div>
                    <h2>
                        <slot name="session-subtitle"></slot>
                    </h2>
                    <p>
                        <slot name="session-description"></slot>
                    </p>
                </div>
                <slot name="session-body"></slot>
            </div>
        </div>
    </section>

</template>

<style scoped>
section {
    padding-top: 10vh;
    padding-bottom: 10vh;
}

.session-title {
    font-size: 17px;
    font-weight: 500;
    line-height: 27.5px;
    text-align: center;
    color: #FFCB45;
}

h2 {

    font-size: 32px;
    font-weight: 700;
    line-height: 40px;
    text-align: center;
}

p {
    font-size: 17px;
    font-weight: 500;
    line-height: 27.5px;
    text-align: center;
}
</style>
