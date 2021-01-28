<template>
  <section id="categories" class="lg:my-12 m-6">
    <div class="max-w-6xl mx-auto">
      <header class="categories-header mb-8 flex">
        <h1 class="text-2xl font-semibold w-1/2">Top Categories</h1>
        <a
          href="categories.html"
          class="text-lg font-semibold w-1/2 mt-1 text-right hover:underline"
          >All Categories</a
        >
      </header>

      <div class="flex flex-wrap text-white categories text-gray-800">
        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/190/390);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              Freelance
            </h3>
          </div>
        </div>

        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/191/391);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              How To
            </h3>
          </div>
        </div>

        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/192/392);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              SEO
            </h3>
          </div>
        </div>

        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/193/393);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              UI design
            </h3>
          </div>
        </div>

        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/194/394);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              UX desing
            </h3>
          </div>
        </div>

        <div class="lg:w-1/6 md:w-1/2 w-full lg:mb-0 mb-16">
          <div
            onclick="window.location='category-page.html'"
            class="cursor-pointer category-card hover:shadow-2xl transition-3 relative h-64 mx-1 inner rounded shadow-lg p-3 bg-cover"
            style="background-image: url(https://picsum.photos/195/395);"
          >
            <h3 class="title text-gray-900 font-semibold text-lg absolute">
              More
            </h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>
