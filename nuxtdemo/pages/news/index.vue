<template>
  <div>
      <h2>News Index page</h2>
       <ul>
        <li><a href="/">Home</a></li>
        <li><nuxt-link :to="{name:'news-id',params:{id:123,title:'i am news'}}">News-1</nuxt-link></li>
      </ul>
  </div>
</template>