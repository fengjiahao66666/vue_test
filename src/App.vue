<template>
	<div class="container">
		<Category title="美食" :listData="foods">
			<img src="../01_src_分析脚手架/assets/logo.png" alt="">
		</Category>
		<Category title="游戏">
			<ul>
              <li v-for="(g,index) in games" :key="index">{{ g }}</li>
            </ul>
        </Category>
		<Category title="电影">
			<video controls src="http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4"></video>
		</Category>
	</div>
</template>

<script>
	import Category from './components/Category.vue'
	export default {
		name:'App',
		components:{Category},
		data() {
			return {
				foods: ['火锅', '烧烤', '小龙虾'], 
				games: ['红色警戒', '穿越火线', '劲舞团'], 
				films: ['《教父》', '《拆弹专家》', '《你好，李焕英》']
			}
		},
	}
</script>

<style scoped>
	.container{
		display: flex;
		justify-content: space-around;
	}
</style>