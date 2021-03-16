<template>
	<view class="content">
		<image class="bg-image" src="/static/bg.png"></image>
		<view class="my-info"></view>
		<view class="uni-flex uni-row">
			<view class="flex-item uni-bg-red" @click="navToVue('../skill/skill')">
				<image class="tag-image" src="/static/item-5.png"></image>
				<view>专业技能</view>
			</view>
			<view class="flex-item uni-bg-green" @click="navToVue('../experience/experience')">
				<image class="tag-image" src="/static/item-6.png"></image>
				<view>项目经验</view>
			</view>
			<view class="flex-item uni-bg-blue" @click="navToVue('../work/work')">
				<image class="tag-image" src="/static/item-7.png"></image>
				<view>工作经历</view>
			</view>
			<view class="flex-item uni-bg-blue" @click="navToVue('../assessment/assessment')">
				<image class="tag-image" src="/static/item-8.png"></image>
				<view>自我评价</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			navToVue(str){
				uni.navigateTo({
					url: str
				});
                // uni.navigateTo({
                //     url:'pages/skill/skill'
                // })
            }
		}
	}
</script>

<style lang="scss">
	.uni-flex{
		display: flex;
		width: 100%;
	}
	.my-info{
		background-color: #fff;
		padding: 20rpx;
		width: 100%;
	}
	.flex-item {
		width: 25%;
		height: 200rpx;
		text-align: center;
		line-height: 200rpx;
		view{
			height: 60rpx;
			line-height: 60rpx;
			font-size: 28rpx;
		}
	}
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.bg-image{
		width: 100%;
	}
	.tag-image{
		width: 100rpx;
		height: 100rpx;
		display: block;
		margin: 0 auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
