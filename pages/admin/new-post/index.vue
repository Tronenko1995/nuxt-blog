<template>
    <NewPostFrom @save="save"/>
</template>

<script>
import NewPostFrom from '@/components/Admin/NewPostFrom.vue'
export default {
    components: { NewPostFrom },
    layout: 'admin',
    methods: {
        save(post) {
            console.log('Post added!', post)
        }
    }
}
</script>