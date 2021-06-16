<template>
	<view class="videoList">
		<view class="swiper-box">
			<swiper class="swiper" :vertical="true">
				<swiper-item v-for="item in videoList" :key="item.id">
					<view class="swiper-item">
						<video-player :src="item.src"></video-player>
					</view>
					<view class="left-box">
						<list-left></list-left>
					</view>
					<view class="right-box">
						<list-right></list-right>
					</view>
				</swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	import videoPlayer from './videoPlayer.vue'
	import listLeft from './listLeft.vue'
	import listRight from './listRight.vue'
	export default {
		props:['list'],
		data() {
			return {
				videoList: []
			};
		},
		watch:{
			list() {
				this.videoList = this.list
			}
		},
		components: {
			videoPlayer,
			listLeft,
			listRight
		}
	}
</script>

<style lang="scss" scoped>
.videoList {
	height: 100%;
	width: 100%;
	.swiper-box {
		width: 100%;
		height: 100%;
		.swiper {
			width: 100%;
			height: 100%;
			.swiper-item {
				width: 100%;
				height: 100%;
				color: #000;
			}
			.left-box {
				z-index: 20;
				position: absolute;
				bottom: 50px;
				left: 10px;
			}
			.right-box {
				z-index: 20;
				position: absolute;
				bottom: 50px;
				right: 10px;
			}
		}
	}
}
</style>
