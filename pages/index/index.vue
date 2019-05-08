<template>
	<view class="page">
		<!-- 轮播块 -->
		<swiper :indicator-dots="true" :autoplay="true" class="carousel">
			<swiper-item>
				<image src="../../static/carousel/batmanvssuperman.png" class="carousel"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/carousel/spiderman.png" class="carousel"></image>
			</swiper-item>
		</swiper>
		
		
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onLoad() {
			uni.request({
				url:"https://www.imovietrailer.com/superhero/index/carousel/list",
				method:"POST",
				header:{
                    'Content-Type': 'application/x-www-form-urlencoded',
                    'charset':'utf-8'
                },
				data:{
					qq:null
				},
				sucess:(response)=>{
					console.log(response.data)
				}
			})
		},
		methods: {

		}
	}
</script>

<style>
	@import url("index.css");
</style>
