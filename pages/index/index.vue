<template>
	<view class="content">
		<first-nav></first-nav>
		<video-list :list="list"></video-list>
		<tab></tab>
	</view>
</template>

<script>
	import tab from '../../components/tab.vue'
	import firstNav from '../../components/first-nav.vue'
	import videoList from '../../components/videoList.vue'
	export default {
		data() {
			return {
				list: []
			}
		},
		components:{
			tab,
			firstNav,
			videoList
		},
		onLoad() {
			
		},
		onLoad() {
			this.getVideos()
		},
		methods: {
			getVideos() {
				uni.request({
					url: 'http://localhost:3000/list',
					success:(res)=> {
						this.list = res.data
						console.log(this.list);
					}
				})
			}
		}
	}
</script>

<style lang="scss" scoped>
	.content {
		height: 100%;
		width: 100%;
	}
</style>
