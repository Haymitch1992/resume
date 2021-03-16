<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style  lang="scss">
	/*每个页面公共css */
	page{
		background: #eee;
		height: 100vh;
	}
	.skill-box{
	  background: #fff;
	  width: 100%;
	  text-align: center;
	  margin: 20rpx 0rpx;
	  border-radius: 16rpx;
	  padding: 30rpx 0;
	}
	.container{
	  padding: 20rpx;
	}
	.skill-list{
		text-align: left;
		padding: 10rpx 20rpx;
		view{
			padding: 10rpx 40rpx;
			position: relative;
		}
		text{
			font-size: 26rpx;
		}
		.dot-text{
			display: inline-block;
			border-radius: 50%;
			border: 6rpx solid #9fbfea;
			box-sizing: border-box;
			background: '#9fbfea';
			margin: 0 20rpx ;
			position: absolute;
			left: -10rpx;
			top: 24rpx;
		}
		.skill-text{
			display: inline-block;
		}
	}
</style>
