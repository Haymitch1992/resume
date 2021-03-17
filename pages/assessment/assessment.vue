<template>
	<view class="container">
	  <view class="skill-box">
		  <modelTitle titleText="自我评价"></modelTitle>
		  <view class="skill-list">
			  <view>
				  <text class="dot-text"></text>
				  <text class="skill-text">注重团队配合、代码规范、有较强的沟通能力，能够迅速了解需求并把控项目进度。</text>
			  </view>	
			  <view>
				  <text class="dot-text"></text>
				  <text class="skill-text">对用户体验、交互操作流程、及用户需求有一定了解。</text>
			  </view>
			<view>
				<text class="dot-text"></text>
				  <text class="skill-text">热爱阅读并关注前端最新技术，善于总结不断积累，更新自己的技术博客。</text>
			</view>	
			<view>
				<text class="dot-text"></text>
			  <text class="skill-text">具有自我解决问题的能力、善于运用新知识，能够适应项目上线的压力。</text>
			</view>
		  </view>
	  </view>
	</view>
</template>

<script>
	import modelTitle from '../../components/model-title/model-title.vue';
	export default{
		components:{
			modelTitle
		},
	}
</script>

<style>
</style>
