<template>
  <div id="app">
    <el-input boolean v-model="ipt1" @blur="changeIpt()"/>
    <el-input boolean v-model="ipt2" @blur="changeIpt()"/>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      h1: '',
      h2: '',
    }
  },
  methods:{
    changeIpt(){
      setTimeout(()=>{
        this.$alert('这是一段内容', '标题名称', {
          confirmButtonText: '确定',
        });
      },100)
    },
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
