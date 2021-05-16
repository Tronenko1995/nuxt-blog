<template>
    <section v-if="comments" class="comments">
        <div class="container">
            <h2 class="title"> Comments: </h2>
            <div class="comment" v-for="(comment, i) in comments" :key="i">
                <p class="name">{{ comment.name }}</p>
                <p class="text">{{ comment.text }}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    props: {
        comments: {
            type: Array,
            default: null
        }
    }
}
</script>

<style lang="scss">
.comments {
    text-align: center;
    margin: 30px auto;
    width: 600px;
}
.comment {
    padding: 20px;
    margin-bottom: 20px;
    background-color: #fff;
    .name {
        font-size: 24px;
        color: #5c4de7;
        margin-bottom: 12px;
    }
}
</style>