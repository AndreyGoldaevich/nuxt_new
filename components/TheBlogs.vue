<template>
  <div id="blog" class="panel box">
    <div class="in">
      <h2>Blog</h2>

      <p>
        Ожидает наполнения
        <a href="#">Новостная рассылка</a>.
      </p>

      <div id="blog_posts">
      </div>

      <!--=== Begin Post Navigation ===-->
      <div class="post-navigation">
        <div class="alignleft older"></div>
        <div class="alignright newer"></div>
      </div>
      <!--=== End Post Navigation ===-->
    </div>
  </div>
</template>

<script>
export default {
  props: {
    blogs: {
      type: [Array],
      required: true
    }
  },

  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('en', options)
    }
  }
}
</script>

<style scoped>
#blog_posts .post {
  width: 100%;
  clear: both;
  float: left;
  padding-top: 40px;
  margin-top: 10px;
  background: url('~assets/images/sep.png') top left repeat-x;
}

#blog_posts .post .post_left {
  width: 35%;
  float: left;
}

#blog_posts .post .post_right {
  width: 60%;
  float: right;
}

.post .post_date h5 {
  color: #777 !important;
}

.post .post_title {
  margin-bottom: 10px;
}

a {
  font-style: normal;
  transition: 250ms;
}

a:hover {
  color: #ff4343;
}

.post .post_thumb,
.post .post_video {
  margin-bottom: 30px;
  overflow: hidden;
}
</style>
