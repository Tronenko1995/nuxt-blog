<template>
  <div class="wrapper-content wrapper-content--fixed">
      <Post :post="post" />
      <Comments :comments="comments" />
      <NewComment />
  </div>
</template>

<script>
import Post from '@/components/Blog/Post.vue'
import Comments from '@/components/Comments/Comments.vue'
import NewComment from '@/components/Comments/NewComment.vue'
export default {
    components: { Post, Comments, NewComment},
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
    }
}
</script>

<style lang="scss">
.post {
    max-width: 900px;
    margin: 0 auto;
}
.post-header {
    text-align: center;
    margin-bottom: 30px;
    img {
        max-width: 400px;
        margin-bottom: 16px;
    }
    p {
        color: #999;
    }
}
.post-body {
    text-align: left;
}
</style>