<template>
  <div class="category">
    <h3>{{title}}</h3>
    <!-- <ul>
        <li v-for="item,index in listData" :key="index">{{ item }}</li>
    </ul> -->
    <!-- 定义一个插槽，等着组件的使用者进行填充 -->
    <slot>我是一个默认者，使用者没传入具体结构时出现</slot>
  </div>
</template>

<script>
export default {
    name:'Categroy',
    props:['title']
}
</script>

<style>
  .category{
    background-color: skyblue;
    width: 200px;
    height: 300px;
  }
  h3{
    text-align: center;
    background-color: orange;
  }
  img{
    width: 100%;
  }
  video{
    width: 100%;
  }
</style>