<template>
  <div>
    <!-- TODO: 路由占位 -->
    <!-- <router-view></router-view> -->

    <my-addition></my-addition>


    <h3>-----------------------------</h3>


    <my-subtraction></my-subtraction>

  </div>
</template>

<script>


// TODO 导入 index 组件
// import index from '@/views/index.vue'

const Addition = () =>
    import ( /* webpackChunkName: "Addition_Subtraction." */ '@/views/Addition.vue')

const Subtraction = () =>
    import ( /* webpackChunkName: "Addition_Subtraction." */ '@/views/Subtraction.vue')



export default {
  data(){
    return {

    }
  },

  components:{
    'my-addition':Addition,
    'my-subtraction':Subtraction
  }
}
</script>

<style></style>
