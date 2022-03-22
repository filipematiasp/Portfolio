<template>
  <div class="q-pa-md row items-start justify-center">
    <q-card class="my-card q-pa-md shadow-2" style="width:80%;height:250px;">
      <q-card-section horizontal>
        <q-card-section class="col-9">
          <div class="text-h6">
            Titulo do artigo, sobre o javascript framework quasar
          </div>
          <div class="text-weight-light" style="color: #26a69a">
            by: Filipe 20/03/2022
          </div>
          <div class="text-body1 q-pt-md" >
            Lorem Ipsum is simply dummy text of the printing andk a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged..
          </div>
        </q-card-section>
        <q-card-section class="col-3">
          <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" style="max-height: 165px"/>
          <q-card-actions align="right">
            <q-btn color="primary" icon-right="arrow_right_alt" label="Ler mais" flat />
          </q-card-actions>
        </q-card-section>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
export default {
  name: "BlogNews",
  props: {
    articleImg: {
      type: String,
      required: true
    },
    articleTitle: {
      type: String,
      required: true
    },
    articleContent: {
      type: String,
      require: true
    }
  }
}
</script>

<style scoped>
</style>
