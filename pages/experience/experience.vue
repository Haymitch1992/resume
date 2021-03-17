<template>
	<view>
		<view class="uni-margin-wrap">
			<swiper class="swiper" circular :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
				<swiper-item>
					<view class="container">
						<view class="skill-box">
							<modelTitle titleText="项目经验"></modelTitle>
							<view class="experience-box">
								<view class="experience-title">亮狮网</view>
								<view>
									<text class="tag-text tag-text-1">Vue</text>
									<text class="tag-text tag-text-2">Element</text>
									<text class="tag-text tag-text-3">Element</text>
									<text class="date-text">2002.2.2</text>
								</view>
								<view class="experience-line">
									该项目是商业地产租赁买卖平台，对外向客户展示房源信息、通过注册登录，可实现在线签约付款并提供管家等增值服务。
								</view>
								<view class="experience-line">
									对内向员工提供楼盘建档、房源上下架管理、销控管理、合同签约、工单的录入跟进和绩效考核等功能。
								</view>
								<view class="skill-list experience-list">
									<view>
										<text class="dot-text"></text>
										<text class="skill-text">用户权限通过Vuex进行管理，确保核心数据按权限查看。</text>
									</view>
									<view>
										<text class="dot-text"></text>
										<text class="skill-text">为提升响应速率将图片信息懒加载。</text>
									</view>
									<view>
										<text class="dot-text"></text>
										<text class="skill-text">根据房源的地理位置调用百度地图API显示附近周边配套设施。</text>
									</view>
									<view>
										<text class="dot-text"></text>
										<text class="skill-text">为整个楼栋信息建档，可添加删除单个楼层或单个房间，各类交互数据和可视化展示。</text>
									</view>

									<view>
										<text class="dot-text"></text>
										<text class="skill-text">熟练使用element-ui的控件，能够很好的与产品、设计、后台沟通协作，高度还原需求。</text>
									</view>
									<view>
										<text class="dot-text"></text>
										<text class="skill-text">使用Momnet对时间进行格式化处理。</text>
									</view>
								</view>
							</view>
						</view>
					</view>
				</swiper-item>
				<swiper-item>
					<view class="container">
						<view class="skill-box">
							<modelTitle titleText="项目经验"></modelTitle>
							<view class="skill-list">
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
							</view>
						</view>
					</view>
				</swiper-item>
				<swiper-item>
					<view class="container">
						<view class="skill-box">
							<modelTitle titleText="项目经验"></modelTitle>
							<view class="skill-list">
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
								<view>
									<text class="dot-text"></text>
									<text class="skill-text">熟练掌握Html5、Css3、Javascript、Ajax</text>
								</view>
							</view>
						</view>
					</view>
				</swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
import modelTitle from '../../components/model-title/model-title.vue';
export default {
	data() {
		return {
			indicatorDots: false,
			autoplay: false,
			interval: 2000,
			duration: 500
		};
	},
	components: {
		modelTitle
	}
};
</script>

<style lang="scss">
.experience-box {
	text-align: left;
	padding: 0 40rpx;
	.experience-title{
		font-size: 40rpx;
		line-height: 80rpx;
	}
	.experience-line{
		font-size: 24rpx;
		line-height: 40rpx;
		padding-top: 20rpx;
	}
	.date-text {
		float: right;
		font-size: 28rpx;
		color: #666;
	}
	.experience-list {
		margin-top: 20rpx;
		background-color: rgb(230, 247, 255);
		.skill-text {
			color: #007aff;
		}
	}
}
.tag-text {
	border: 2rpx solid #42b783;
	margin: 0 10rpx 0 0;
	padding: 4rpx 10rpx;
	font-size: 24rpx;
	color: #42b783;
}
.tag-text-2 {
	border: 2rpx solid #f89f5b;
	color: #f89f5b;
}
.tag-text-3 {
	border: 2rpx solid #f78070;
	color: #f78070;
}
.tag-text-1 {
	border: 2rpx solid #42b783;
	color: #42b783;
}

.swiper {
	height: 100vh;
}
</style>
