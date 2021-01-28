<template>
  <div>
    <Nav></Nav>

    <Featured></Featured>

    <Categories></Categories>

    <ContentList></ContentList>

    <Footer></Footer>
  </div>
</template>

<script>
import Nav from "./Nav";
import Featured from "./Featured";
import Categories from "./Categories";
import ContentList from "./ContentList";
import Footer from "./Footer";
export default {
  name: "Layout",
  components: {
    Nav,
    Featured,
    Categories,
    ContentList,
    Footer,
  },
};
</script>
