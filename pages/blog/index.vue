<template>
  <div class="wrapper-content wrapper-content--fixed">
    <Intro title="My posts:" />
    <PostsList :posts="posts" />
  </div>
</template>
 
<script>
export default {
  data () {
    return {
      posts: [
        {
          id: 1,
          title: '1 post',
          descr: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem necessitatibus eum quibusdam animi officiis perspiciatis distinctio, quis beatae similique harum.',
          img: 'https://kubnews.ru/upload/iblock/21d/21de27a6fcd2d0e93149fd84b6d3266e.jpg'
        },
        {
          id: 2,
          title: '2 post',
          descr: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis deleniti in libero expedita, repellendus modi!',
          img: 'https://zoomagazin.dp.ua/image/catalog/blog-img/ponos.jpg'
        },
        {
          id: 3,
          title: '3 post',
          descr: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam, quod sint. Quas deserunt esse repellat iusto libero voluptas! Qui, vero!',
          img: 'https://www.purinaone.ru/dog/sites/purinaonedog.ru/files/2019-08/m_8.jpg'
        },
      ]
    }
  }
}
</script>
