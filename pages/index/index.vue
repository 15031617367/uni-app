<template>
	<view class="page">
		<!-- 轮播块 -->
		<swiper :indicator-dots="true" :autoplay="true" class="carousel">
			<swiper-item>
				<image src="../../static/carousel/batmanvssuperman.png" class="carousel"></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/carousel/spiderman.png" mode="" class="carousel"></image>
			</swiper-item>
		</swiper>
		
		<!-- 热门超英 -->
		<view class="page-block super-hot">
			<view  class="hot-title-wapper">
				<image src="../../static/icos/hot.png" mode="" class="hot-ico"></image>
				<view  class="hot-title">
					热门超英
				</view>
			</view>
			<scroll-view scroll-x class="page-block hot">
				<view class="single-poster">
					<view class="post-wapper">
						<image src="../../static/poster/civilwar.jpg" mode="" class="poster"></image>
						<view class="movie-name">复仇者联盟3</view>
						<view>
							<view class="left">
								<uni-rate max="5" value="4.9" disabled="true" size="14" margin="0" class="star-ico"></uni-rate>
							</view>
							<view class="movie-score maging_left right">4.9</view>
						</view>
					</view>
				</view>
				<view class="single-poster">
					<view class="post-wapper">
						<image src="../../static/poster/justice.png" mode="" class="poster"></image>
						<view class="movie-name">正义联盟</view>
						<view>
							<view class="left">
								<uni-rate max="5" value="4.9" disabled="true" size="14" margin="0" class="star-ico"></uni-rate>
							</view>
							<view class="movie-score maging_left right">4.9</view>
						</view>
					</view>
				</view>	
			</scroll-view>
		</view>
		<!-- 热门预告 -->
		<view class="page-block super-hot">
			<view  class="hot-title-wapper">
				<image src="../../static/icos/interest.png" mode="" class="hot-ico"></image>
				<view  class="hot-title">
					热门预告
				</view>
			</view>
			<view class="video">
				<video class="video" src="http://valipl.cp31.ott.cibntv.net/6974532859B3B717EF7DA2B86/03000801005CB932D0BC604003E8806EE107E3-99A8-4203-8808-ACF3D31E232A.mp4?ccode=0502&duration=163&expire=18000&psid=83a5fa07d759307415c073e03882e4ce&ups_client_netip=7b3af907&ups_ts=1557821640&ups_userid=&utid=2IBIFSkCjGsCAXs6%2BQfZ43PN&vid=XMzU2MTQyOTE2NA%3D%3D&vkey=Ab23b601901d010d46e2ffce85fe2d698"
					   poster="https://r1.ykimg.com/054101015CD592F58B6C068FCC945443"></video>
			</view>
		</view>
		<!-- 猜你喜欢 -->
		<view class="page-block super-hot">
			<view  class="hot-title-wapper">
				<image src="../../static/icos/guess-u-like.png" mode="" class="hot-ico"></image>
				<view  class="hot-title">
					猜你喜欢
				</view>
			</view>
			<view>
				<view class="list">
					<view>
						<image src="../../static/poster/civilwar.jpg" mode="" class="poster"></image>
					</view>
					<view class="explain_view">
						<view>美国队长3</view>
						<view>
							<uni-rate max="5" value="4.9" disabled="true" size="14" margin="0" class="star-ico"></uni-rate>
						</view>
						<view class="explain">
							<view>2018/美国/科幻/超级英雄 </view>
							<view>上映时间：2012-05-06（中国）</view>
						</view>
					</view>
					<view class="fabulous_view">
						<view class="">
							<view >
								<image src="../../static/icos/praise.png" mode="" class="fabulous_img"></image>
							</view>
							
						</view>
						<view class="fabulous_text">
							赞一下
						</view>
					</view>
					
				</view>
				
				
				
			</view>
			
		</view>
		
			
			
			
			
			
	</view>
</template>

<script>
	import uniRate from "../../components/uni-rate/uni-rate.vue"
	export default {
		data() {
			return {
				url:'',
				carouselList:null,
				hotSuperheroList:null
			}
		},
		onLoad() {
			
		},
		methods: {
		},
		components: {uniRate}
	}
</script>

<style>
	@import url("index.css");
	.left{
		float: left;
		margin-right: 5upx;
	}
	.right{
		float: right;
		margin-right: 10upx;
	}
	.test{
		width: 100%;
		height: 600px;
	}
	.video{
		width: 100%;
		height: 400upx;
	}
	/* 猜你喜欢 */
	.list{	
		display: flex;
	}
	.explain_view{
		margin-left: 10upx;
	}
	.explain{
		font-size: 12px;
		color:#808080
	}
	.fabulous_view{
		width: 20%;
		border-left: 1px #808080 dashed;
		display: flex;
		flex-direction:column;
		justify-content:center;
		align-items: center;
	}
	.fabulous_img{
		width: 92upx;
		height: 92upx;
	}
	.fabulous_text{
		color:#ffc234
	}

</style>
