<template>
  <section id="latest" class="lg:my-12 lg:mt-24 m-6">
    <div class="max-w-6xl mx-auto">
      <div class="flex flex-wrap categories">
        <div class="lg:w-2/3 w-full">
          <articles></articles>
          <!-- most-recent-wrapper -->
        </div>

        <div class="lg:w-1/3 w-full px-4">
          <blog-posts></blog-posts>
          <!-- popular-wrapper -->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BlogPosts from './BlogPosts'
import Articles from './Articles'
export default {
  components: {BlogPosts, Articles}
};
</script>
