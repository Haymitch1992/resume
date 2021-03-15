<template>
	<view>
	  <text class="line"></text>
	  <text class="circle"></text>
	  <text class="model-Title">
		{{titleText}}
	  </text>
	  <text class="circle"></text>
	  <text class="line"></text>
	</view>
</template>

<script>
	export default {
		props:{
			titleText:String
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.model-Title{
	  color: #7e4151;
	  display: inline-block;
	  font-size: 32rpx;
	}
	.circle{
	  width: 14rpx;
	  height: 14rpx;
	  border: 4rpx solid #9fbfea;
	  display: inline-block;
	  border-radius: 50%;
	  margin: 0 20rpx;
	}
	.line{
	  width: 60rpx;
	  height: 4rpx;
	  background-color: #9fbfea;
	  display: inline-block;
	  position: relative;
	  top: -8rpx;
	}
</style>
