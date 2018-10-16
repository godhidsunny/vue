<template>
  <footer>
      <p>{{copyright}} {{title}}</p>
  </footer>
</template>

<script>
export default {
  name: 'app-footer',
  props:{
    title:{
      type:String
    }
  },
  data () {
    return {
      copyright:"Copyright Vue 2.0"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer{background:lightcoral;
text-align: center;
padding: 10px;}
</style>
