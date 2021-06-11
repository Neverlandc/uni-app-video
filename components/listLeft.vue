<template>
	<view class="listLeft">
		<view class="author">
			撒大声地
		</view>
		<view class="title">
			阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放阿达发放
		</view>
		<view class="music">
			奥术大师大所多
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
	.listLeft {
		height: 150px;
		margin-left: 10px;
		color: #fff;
		width: 150px;
		.author{
			height: 35px;
			line-height: 35px;
			font-size: 15px;
		}
		.title {
			max-height: 60px;
			line-height: 20px;
			font-size: 12px;
			width: 100%;
			word-wrap: break-word;
			overflow: hidden;
			word-break: break-all;  /* break-all(允许在单词内换行。) */
			text-overflow: ellipsis;  /* 超出部分省略号 */
			display: -webkit-box; /** 对象作为伸缩盒子模型显示 **/
			-webkit-box-orient: vertical; /** 设置或检索伸缩盒对象的子元素的排列方式 **/
			-webkit-line-clamp: 3; /** 显示的行数 **/
		}
		.music {
			height: 35px;
			line-height: 35px;
			font-size: 12px;
		}
	}
</style>
