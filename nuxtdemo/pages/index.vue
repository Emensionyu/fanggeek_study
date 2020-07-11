<template>
  <div>
    <div class="dist">
      <img src="~static/mai.jpg" alt="">
    </div>
      <h2>News Index page</h2>
      <p>NewsID:{{$route.params.newsId}}</p>
       <ul>
        <li><a href="/">Home</a></li>
        <li><nuxt-link :to="{name:'about'}">about</nuxt-link></li>
        <li><nuxt-link :to="{name:'news'}">news</nuxt-link></li>

      </ul>
  </div>
</template>

<script>

export default {
  components: {

  }
}
</script>

<style>

</style>