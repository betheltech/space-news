<template>
  <div class="popular-wrapper">
    <div class="flex flex-wrap text-gray-900 mb-6">
      <h3 class="text-2xl font-semibold">Blog Posts</h3>
    </div>

    <div class="popular-item mb-10" v-for="(post, key) in posts.docs" :key="key">
      <div class="flex">
        <div class="w-1/3 lg:text-center">
          <span class="text-3xl font-light text-gray-300">{{ key }}</span>
        </div>
        <div class="w-full text-gray-400">
          <h3 class="text-normal font-semibold leading-tight text-gray-900">
            <a :href="post.url" target="_blank">
              {{ post.title }}
            </a>
          </h3>
          <div class="inner-info text-sm text-gray-700 mt-1">
            <span class="item-created-on">{{ post.published_date | moment("MMMM Do, YYYY")  }}</span>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
/* eslint-disable */
import axios from 'axios'
import moment from 'moment'
export default {
  data() {
    return {
      posts: []
    }
  },
  mounted() {
    axios.get('https://spaceflightnewsapi.net/api/v1/blogs?limit=5')
    .then(response => this.posts = response.data)
    .catch(error => console.log(error))
  },
};
</script>
