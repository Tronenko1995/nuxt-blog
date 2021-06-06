<template>
    <section class="new-comment">
        <div class="container">
            <h2 class="title"> New Comment! </h2>
            <Message v-if="message" :message="message" />
            <form @submit.prevent="onSubmit" class="contact-form">
                <AppInput v-model="comment.name" type="text"> Name: </AppInput>
                <AppTextArea v-model="comment.text" type="text"> Text: </AppTextArea>
                <div class="controls">
                    <AppButton class="btnWhite"> Submit! </AppButton>
                </div>
            </form>
        </div>
    </section>
</template>

<script>
export default {
    data () {
        return {
            message: null,
            comment: {
                name: '',
                text: ''
            }
        }
    },
    methods: {
        onSubmit () {
            this.message = 'Submited!'
            console.log(this.comment)
        }
    }
}
</script>

<style lang="scss">
.new-comment {
    text-align: center;
    .contact-form {
        max-width: 600px;
        margin: 30px auto;
    }
    .controls {
        margin: 30px auto;
    }

}
</style>