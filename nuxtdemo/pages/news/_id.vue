<template>
  <div>
      <h2>News-Content [{{$route.params.id}}]</h2>
      <ul>
        <li><a href="/">Home</a></li>
        <li><nuxt-link :to="{name:'home'}">home</nuxt-link></li>
      </ul>
  </div>
</template>
<script>
export default {
  // 动态参数校验
   validate ({ params }) {
    // Must be a number
    return /^\d+$/.test(params.id)
  },
  data(){
    return{
      title:this.$route.params.title
    }
  },
  // 
  head(){
    return{
      title:this.title,
      meta:[
        {hid:'description',name:'new1',content:'this is news'}
      ]
    }
  }
}
</script>
