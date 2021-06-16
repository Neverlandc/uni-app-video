<template>
	<view class="listRight">
		<view class="author-img">
			<image class="img" src="../static/img/author.jpg" mode=""></image>
			<view class="iconfont icon-jiahao add" v-show="showFollow" @click="follow">
				
			</view>
		</view>
		<view class="iconfont icon-aixin right-box" :style="aixinStyle" @click="aixinClick">
			
		</view>
		<view class="number">
			123
		</view>
		<view class="iconfont icon-pinglun right-box">
			
		</view>
		<view class="number">
			123
		</view>
		<view class="iconfont icon-zhuanfa right-box">
			
		</view>
		<view class="number">
			123
		</view>
		<view class="around">
			<image class="img" src="../static/img/around.jpg"></image>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				showFollow: true,
				aixinStyle: ''
			};
		},
		methods:{
			follow() {
				this.showFollow = false
			},
			aixinClick() {
				this.aixinStyle = this.aixinStyle === '' ? 'color: red;' : ''
			}
		}
	}
</script>

<style lang="scss" scoped>
	.listRight {
		width: 50px;
		margin: 0 auto;
		.author-img {
			height: 50px;
			width: 50px;
			border-radius: 50%;
			border: 2px solid #fff;
			position: relative;
		}
		.img {
			height: 50px;
			width: 50px;
			border-radius: 50%;
		}
		.right-box {
			width: 50px;
			height: 40px;
			margin-top: 10px;
			text-align: center;
			line-height: 40px;
			color: #fff;
			font-size: 33px;
		}
		.number {
			font-size: 12px;
			text-align: center;
			color: #fff;
		}
		.around {
			height: 50px;
			width: 50px;
			margin-top: 10px;
			animation: CDrotate 3s linear 0.2s infinite;
		}
		.add {
			width: 18px;
			height: 18px;
			border-radius: 50%;
			background: red;
			position: absolute;
			bottom: -9px;
			left: 16px;
			text-align: center;
			line-height: 18px;
			color: #fff;
			font-size: 10px;
		}
	}
	
@keyframes CDrotate {
	0% {
		transform: rotate(0deg);
	}
	100% {
		transform: rotate(360deg);
	}
}
</style>
