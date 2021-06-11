<template>
	<view class="videoPlayer">
		<video class="video" :autoplay="true" :loop="true" :src="src" :controls="false"></video>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		},
		props: ['src']
	}
</script>

<style lang="scss" scoped>
	.videoPlayer {
		width: 100%;
		height: 100%;
		.video {
			width: 100%;
			height: 100%;
		}
	}
</style>
