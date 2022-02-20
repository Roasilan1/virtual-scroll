<template>
  <List  :list="list" :itemHeight="60"/>
</template>
<script>
import List from "@/components/List/List";
export default {
  components:{
    List
  },
  data(){
    return {
      list:[]
    }
  },
  methods: {
    //初始化列表 ，循环渲染 500条
    initList(){
      for(let i=0;i<500;i++){
        this.list.push(i);
      }
    },

  },
  mounted() {
    this.initList();
  },
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}

</style>
