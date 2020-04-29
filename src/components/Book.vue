<template>
      <div class="card border border-dark rounded">
        <h4 class="text-center card-title">{{book.title}}</h4>
        <p class="text-center card-text">{{book.author}}</p>
        <img class="card-img img-fluid d-flex" :src="book.img" />
      </div>
</template>

<script>
  export default {
    name: 'Book',
    props: { book: Object },
  }
</script>

<style scoped>

</style>
