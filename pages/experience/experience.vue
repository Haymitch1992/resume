<template>
	<view >
		<view class="uni-margin-wrap">
			<swiper class="swiper" circular :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
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
	export default{
		data(){
			return{
				indicatorDots: false,
				autoplay: false,
				interval: 2000,
				duration: 500
			}
		},
		components:{
			modelTitle
		},
	}
</script>

<style>
	.swiper{
		height: 100vh;
	}
</style>
