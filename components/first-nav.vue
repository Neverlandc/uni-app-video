<template>
	<view class="firstNav">
		<view class="iconfont icon-sousuo icon">
			
		</view>
		<view class="middle">
			<view class="text">
				推荐
			</view>
			<view class="text">
				<view class="iconfont icon-vertical_line icon-shuxian"></view>
			</view>
			<view class="text">
				同城
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss" scoped>
.firstNav {
	width: 100%;
	position: fixed;
	top: 25px;
	left: 0;
	height: 35px;
	line-height: 35px;
	margin: 0 auto;
	// background: #000;
	z-index: 9;
	.icon {
		position: absolute;
		top: 0;
		left: 0;
		color: #fff;
		width: 20%;
		text-align: center;
		font-size: 20px;
	}
	.middle {
		text-align: center;
		.text {
			display: inline-block;
			color: #fff;
			margin: 0 10px;
		}
	}
}
</style>
