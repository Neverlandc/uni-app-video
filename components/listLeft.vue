<template>
	<view class="listLeft">
		<view class="author">
			撒野
		</view>
		<view class="title">
			我一脚踏空，我就要飞起来了 我向上是迷茫，我向下听见你说这世界是空荡荡 你说一二三，打碎了过往，消亡 有风吹，破了的归途，你有没有听见我在唱 你说一二三转身，你听被抹掉的慌张 我想，抬头暖阳春草，你给我简单拥抱
		</view>
		<view class="music-box">
			<view class="music">
				撒野 - 凯瑟喵
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
		.music-box {
			width: 100px;
			overflow: hidden;
		}
		.music {
			height: 35px;
			line-height: 35px;
			// width: 150px;
			font-size: 12px;
			animation: music 4s linear 0.2s infinite;
		}
	}
	@keyframes music {
		0% {
			transform: translate3d(80%,0,0);
		}
		100% {
			transform: translate3d(-80%,0,0);
		}
	}
</style>
