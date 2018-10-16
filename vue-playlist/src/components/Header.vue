<template>
  <header v-on:click="changeTitle">
      <h1>{{title1}} {{title}}</h1>
  </header>
</template>

<script>
export default {
  name: 'app-header',
  props:{
    title:{
      type:String
    }
  },
  data () {
    return {
      title1:"Vue.js Demo"
    }
  },
  methods:{
    changeTitle:function(){
      this.title="changed";
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{background: lightgreen;
text-align: center;
padding: 10px;}
</style>
