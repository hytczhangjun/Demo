<template>
  <div class="hello">
    <h1 @click="handleHello">{{ msg }}</h1>
    
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      
    }
  },
  props:['msg'],
  methods: {
    handleHello(){
      this.$emit('increment')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
