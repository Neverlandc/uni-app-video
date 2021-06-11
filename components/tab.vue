<template>
	<view class="tab">
		<view class="tab-box">
			主页
		</view>
		<view class="tab-box">
			关注
		</view>
		<view class="tab-box">
			<view class="iconfont icon-jiahao icon-box"></view>
		</view>
		<view class="tab-box">
			消息
		</view>
		<view class="tab-box">
			我的
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
	.tab {
		height: 50px;
		width: 100%;
		position: fixed;
		bottom: 0;
		left: 0;
		display: flex;
		justify-content: space-around;
		align-items: center;
		.tab-box {
			width: 20%;
			line-height: 50px;
			color: #FFFFFF;
			// background: #000;
			text-align: center;
		}
		.icon-box {
			width: 60%;
			height: 30px;
			background: #fff;
			color: #676767;
			margin: 10px 20%;
			line-height: 30px;
			border-radius: 5px;
			font-size: 15px;
		}
	}
</style>
