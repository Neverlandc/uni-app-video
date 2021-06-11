<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
			uni.hideTabBar()
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="scss">
	html,body {
		width: 100%;
		height: 100%;
	}
	/*每个页面公共css */
	@font-face {
	  font-family: "iconfont"; /* Project id 2602531 */
	  src: url('iconfont/iconfont.woff2?t=1623223288731') format('woff2'),
	       url('iconfont/iconfont.woff?t=1623223288731') format('woff'),
	       url('iconfont/iconfont.ttf?t=1623223288731') format('truetype');
	}
	
	.iconfont {
	  font-family: "iconfont" !important;
	  font-size: 16px;
	  font-style: normal;
	  -webkit-font-smoothing: antialiased;
	  -moz-osx-font-smoothing: grayscale;
	}
	
	.icon-vertical_line:before {
	  content: "\e63a";
	}
	
	.icon-fanhui:before {
	  content: "\e601";
	}
	
	.icon-jiahao:before {
	  content: "\e879";
	}
	
	.icon-sousuo:before {
	  content: "\e62c";
	}
</style>
