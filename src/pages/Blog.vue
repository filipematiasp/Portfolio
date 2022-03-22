<template>
  <div class="text-h3 q-pa-md" style="color: #1976d2">Artigos</div>
  <BlogNews
    article-img="https://cdn.quasar.dev/img/parallax2.jpg"
    article-content="Lorem Ipsum is simply dummy text of the printing andk a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.."
    article-title="Titulo do artigo, sobre o javascript framework quasar"
  />
  <BlogNews />
  <BlogNews />
</template>

<script>
import BlogNews from "components/BlogNews";

export default {
  name: "Blog",
  components: {
    BlogNews
  }


}
</script>

<style scoped>


</style>
