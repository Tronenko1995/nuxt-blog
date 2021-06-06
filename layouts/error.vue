<template>
    <section class="not-found">
        <div class="container">
            <div class="not-found__wrapper">
                <p class="title">Page Not Found</p>
                <nuxt-link to="/"> Back to main page </nuxt-link>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.not-found__wrapper {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 80vh;
    width: 100%;
    flex-direction: column;
}
</style>