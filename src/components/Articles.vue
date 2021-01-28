<template>
  <div class="most-recent-wrapper">
    <div class="flex flex-wrap text-gray-900 mb-6">
      <h3 class="text-2xl font-semibold">Recent Articles</h3>
    </div>

    <div class="flex flex-wrap most-recent-item pr-5 mb-10" v-for="(article, key) in articles.docs" :key="key">
      <div class="sm:w-2/3 w-full">
        <div class="most-recent-item-info">
          <div class="catg">
            <!-- <span class="text-xs text-gray-500 uppercase">Editor's Pick</span> -->
          </div>
          <h2
            class="text-normal font-semibold text-gray-900 leading-tight mb-3 mt-1"
          >
            <a :href="article.url" target="_blank">{{ article.title }}</a>
          </h2>
          <p class="text-gray-600 text-sm">
            <span class="item-created-on">{{ article.published_date | moment("dddd, MMMM Do YYYY")  }}</span> - Tags: {{ article.tags.join([', ']) }}
          </p>
        </div>
        <!-- most-recent-item-info -->
      </div>

      <div class="sm:w-1/3 w-full sm:h-auto h-64 sm:mt-0 mt-3 bg-gray-100 rounded overflow-hidden" >
        <img :src="article.featured_image" >
      </div>
    </div>


    <!-- pagination -->
    <div class="most-recent-items-pagination pagination py-5">
      <ul>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >Previews</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >1</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >2</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >3</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >4</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >5</a
          >
        </li>
        <li class="inline-block">
          <a
            class="border border-gray-300 px-3 py-1 rounded hover:bg-gray-800 hover:text-white"
            href=""
            >Next</a
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import axios from 'axios';
export default {
  data() {
    return {
      articles: []
    }
  },

  mounted() {
    axios.get('https://spaceflightnewsapi.net/api/v1/articles')
    .then(response => this.articles = response.data)
    .catch(error => console.log(error))
  },
};
</script>
