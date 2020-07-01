<template>
  <div class="top">
      <a class="button" @click="left">三</a>
      <p>通观预览</p>
      </div>
</template>

<script>

export default {
  name: 'Mainf',
  methods:{
      left(){
          console.log("1");
      }
  }
}
</script>
<style scpoed lang="scss">
.top{
    width:100%;
    height: 2.5rem;
    background:#797272;
    vertical-align: middle;
    line-height: 2.5rem;
    p{
        margin-right: 10px;
    }
}
.button{
    width:2rem;
    height:80%;
    float:left;
    text-align: center;
}
</style>