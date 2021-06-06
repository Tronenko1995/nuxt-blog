<template>
    <div class="message" :class="mesClass">
        {{ message }}
    </div>
</template>

<script>
export default {
    props: {
        mesClass: {
            type: String,
            default: 'success'
        },
        message: {
            type: String,
            required: true
        }
    }
}
</script>

<style lang="scss">
.message {
    &.success {
        color: #26de81;
    }
    &.error {
        color: #fc5c65;
    }
}
</style>