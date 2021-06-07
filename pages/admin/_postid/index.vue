<template>
    <NewPostFrom
    :postEdit="post"
    @save="save"/>
</template>

<script>
import NewPostFrom from '@/components/Admin/NewPostFrom.vue'
export default {
    components: { NewPostFrom },
    layout: 'admin',
    data () {
        return {
            post: {
                id: 1,
                title: '1 post',
                descr: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem necessitatibus eum quibusdam animi officiis perspiciatis distinctio, quis beatae similique harum.',
                img: 'https://kubnews.ru/upload/iblock/21d/21de27a6fcd2d0e93149fd84b6d3266e.jpg',
                content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa facere quibusdam earum alias dolores modi maiores suscipit laboriosam quasi ullam, nostrum optio totam adipisci. Voluptatum pariatur aspernatur distinctio unde mollitia veniam deserunt dicta, asperiores reiciendis nam natus! Distinctio, tenetur nam cum cumque eveniet repudiandae exercitationem a quis laudantium nisi unde.'
            },
            comments: [
                { name: 'Alex', text: 'uidem necessitatibus eum quibusdam animi officiis'},
                { name: 'Eugene', text: 'uidem necessitatibus eum quibusdam animi officiis'}
            ]
        }
    },
    methods: {
        save(post) {
            console.log('Post edit!', post)
        }
    }
}
</script>