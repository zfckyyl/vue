<template>
<div>
  <div class="top">
      <a class="button" @click="left">三</a>
      <p>通观预览</p>
      </div>
      <look1 :he="{..look1style(1)}" style="margin-top:2.6rem;"/>
      <look1 :he="6"/>
      <look1 :he="6"/>
      <look1 :he="4"/>
      <look1 :he="4"/>
      <look1 :he="4"/>
      <look1 :he="4"/>
      <look1 :he="4"/>
      </div>
</template>

<script>
import look1 from '../components/look1.vue'
export default {
  name: 'Mainf',
  components:{
      look1,
  },
  methods:{
      left(){
          console.log("1");
      },
      look1style(id){
          let size,color;
          if(id==1){
              size=6;
              color="#ee7b6e";
          }
          return {
              "size":size,
              "color":color,
          };
      }
  }
}
</script>
<style scpoed lang="scss">
.top{
    width:100%;
    height: 2.5rem;
    background:#797272;
    line-height: 2.5rem;
    text-align:center;
    position: fixed;
    top:0;
    p{
        position: relative;
        top:-1rem;
        left:-1rem;
    }
}
.button{
    width:2rem;
    height:80%;
    float:left;
    text-align: center;
}
</style>
