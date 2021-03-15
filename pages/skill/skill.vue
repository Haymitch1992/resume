<template>
	<view class="container">
	  <view class="skill-box">
		  <modelTitle titleText="专业技能"></modelTitle>
		  <view class="echarts-box">
		  	<view class="echarts-item">1</view>
		  	<view>1</view>
		  	<view>1</view>
		  	<view>1</view>
		  </view>

	  </view>
	  <view class="skill-box">
		  <modelTitle titleText="专业技能"></modelTitle>
	  </view>
	</view>
</template>

<script>
	import modelTitle from '../../components/model-title/model-title.vue'
	export default {
		components:{
			modelTitle
		},
		data() {
			return {
				title: '专业技能'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.skill-box{
	  background: #fff;
	  width: 100%;
	  text-align: center;
	  margin: 10rpx 0rpx;
	  border-radius: 16rpx;
	  padding: 30rpx 0;
	}
	.container{
	  padding: 20rpx;
	}
	.echarts-box{
		display:grid;
		grid-template-columns: 40vw 40vw;
		grid-template-rows: 40vw 40vw;
		justify-content: center;
		.echarts-item{
			color: #0000FF;
		}
	}
</style>
