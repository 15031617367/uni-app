<template>
	<view class="">
		<view class="padding">
			<view class="ico_view">
				<image src="../../static/icos/search.png" mode="" class="ico"></image>
			</view>
			<input class="uni-input" confirm-type="search" placeholder="请输入电影名称" />
		</view>
		<view class="list_view">
			<image src="../../static/poster/civilwar.jpg" mode="" class="poster position"></image>
			<image src="../../static/poster/justice.png" mode="" class="poster position"></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.padding{
		margin-left: 20upx;
		margin-right: 20upx;
		background: #eeeeee;
		display: flex;
	}
	.ico_view{
		width: auto;
		height: 60upx;
		display: flex;
		justify-content:center;
		align-items: center;
		margin-right: 10upx;
		margin-left: 10upx;
	}
	.ico{
		width: 36upx;
		height: 36upx;
	}
	.list_view{
		display:flex;
		flex-wrap:wrap 
	}
	.poster{
		width: 200upx;
		height: 270upx;
	}
	.position{
		margin: 10upx;
	}
</style>
