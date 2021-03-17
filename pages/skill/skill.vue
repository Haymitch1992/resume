<template>
	<view class="container">
	  <view class="skill-box">
		  <modelTitle titleText="技术能力" @click.native="test()"></modelTitle>
		  <view class="echarts-box">
		  	<view class="echarts-item">
			   <canvas style="width: 100%; height: 100%;"  canvas-id="canvas1" id="canvas1"></canvas>
			</view>
		  	<view>
				<canvas style="width: 100%; height: 100%;"  canvas-id="canvas2" id="canvas2"></canvas>
			</view>
		  	<view>
				<canvas style="width: 100%; height: 100%;"  canvas-id="canvas3" id="canvas3"></canvas>
			</view>
		  	<view>
				<canvas style="width: 100%; height: 100%;"  canvas-id="canvas4" id="canvas4"></canvas>
			</view>
		  </view>
	  </view>
	  <view class="skill-box">
		  <modelTitle titleText="专业技能"></modelTitle>
		  <view class="skill-list">
			  <view>
				  <text class="dot-text"></text>
				  <text class="skill-text">熟练掌握HTML5、CSS3、JavaScript、Ajax，能够敏捷开发并高度还原原型效果</text>
			  </view>	
			  <view>
				  <text class="dot-text"></text>
				  <text class="skill-text">熟练掌握Vue.js、ElementUI、IView、BootStarp、Jquery等主流前端框架</text>
			  </view>
			<view>
				<text class="dot-text"></text>
				  <text class="skill-text">熟练掌握Echarts、Axios、Animate、Qrcode、Lodash、Moment等前端组件库</text>
			</view>	
			<view>
				<text class="dot-text"></text>
			  <text class="skill-text">熟练使用git管理工具，熟悉Bower、webpack、Babel、less等前端开发工具</text>
			</view>
			<view>
				<text class="dot-text"></text>
				<text class="skill-text">了解HTML5+VUE的APP混合开发、了解微信小程序开发</text>
			</view>
		  </view>
	  </view>
	</view>
</template>

<script>
	import modelTitle from '../../components/model-title/model-title.vue';
	export default {
		methods: {
			drawProgressBar(id,color,limit,textStr){
				let context = uni.createCanvasContext(id)
				// 文字	
				let num =0
				let timer = setInterval(()=>{
					if(num>=100){clearInterval(timer)}else{
						// 内圈	
						context.beginPath();
						context.arc(this.canvasWidth, this.canvasWidth, this.canvasWidth-30, 0, Math.PI*2);
						context.lineWidth="10"
						context.strokeStyle  = '#eee';
						context.stroke();
						// 外圈
						num ++;
						context.beginPath();
						let arcNum = parseFloat(num/100).toFixed(2)
						context.arc(this.canvasWidth, this.canvasWidth, this.canvasWidth-30, 1.5*Math.PI, 1.5*limit*arcNum*Math.PI);
						context.lineWidth="10"
						context.strokeStyle  = color;
						context.stroke();
						let text = parseInt(((limit*arcNum).toFixed(2))*100)
						
						context.font="28px Georgia";
						context.fillStyle = color
						context.textAlign = 'center';
						context.fillText(text,this.canvasWidth,this.canvasWidth*1.1);
						
						context.font="14px Georgia";
						context.fillStyle= '#666'
						context.textAlign = 'center';
						context.fillText(textStr,this.canvasWidth, this.canvasWidth*2);
						context.stroke();
						context.draw()
					}
				},30)
			}
		},
		components:{
			modelTitle
		},
		data() {
			return {
				title: '专业技能',
				canvasWidth:'100'
			}
		},
		onLoad() {
			let _this = this;
			wx.getSystemInfo({//获取手机系统信息
			  success(res) {
				_this.canvasWidth = (res.windowWidth*.4/2).toFixed(2)
				_this.screenSize = res.windowWidth/750
				console.log(_this.canvasWidth)
			  }
			})
			this.drawProgressBar('canvas1','#fbd75e',.92,'HTML')
			this.drawProgressBar('canvas2','#f89f5b',.82,'CSS')
			this.drawProgressBar('canvas3','#f78070',.74,'JS')
			this.drawProgressBar('canvas4','#42b783',.88,'VUE')
			
				
		}
	}
</script>

<style lang="scss">

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
