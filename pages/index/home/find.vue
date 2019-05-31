<!-- html部分 -->
<template>
	<div id="app">
		<view>
			<view class="top">
				<view class="topdiv2">
					<text class="toptext">今日精品设计案例</text>
					<text class="toptext1">查看更多></text>
				</view>
				<view>
					<wlp></wlp>
					<text class="wlpxia1">Simple Life 【中海锦龙湾】</text><br>
					<text class="wlpxia2">88m²</text>
					<text class="wlpxia2">/</text>
					<text class="wlpxia2">瓯北</text>
					<text class="wlpxia2">|</text>
					<text class="wlpxia2">哇哈设计</text>
				</view>
			</view>
			<view class="top">
				<view class="topdiv2">
					<text class="toptext">视频学会装修</text>
					
					<text class="toptext5">查看更多></text><br>
					<text class="wlpxia5">五分钟学会装修之美</text>
				</view>
				<view  class="top5"></view>
				<view>
					<wlp2></wlp2>
					<text class="wlpxia1">【秒懂装修】什么是新中式风格?最爱新中式,大美中国风</text><br>
					
					<text class="wlpxia2">新中式风格,独具中国文化底蕴和东方之美</text>
				</view>
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			<view class="bottom">
				<image src="../../../static/imgs/13.jpg"></image>
				<view class="ccc">
					<text class="wlpxia1">【秒懂装修】装修防水要做好,闭水试验不能少</text>
				</view>
				
			</view>
			
		</view>
	</div>
</template>
<!-- js部分 -->
<script>
	import wlp from '@/components/wlp-swiper-banner/wlp-swiper-banner2.vue';
	import wlp2 from '@/components/wlp-swiper-banner/wlp-swiper-banner3.vue';
	export default {
		components:{wlp,wlp2},
		name:'',
		data() {
			return {
				
			};
		},
		methods:{
			
		}
	}
</script>
<!-- css部分 -->
<style>
.toptext{
	font-weight:600;
	font-size:35upx;
}
.topdiv2{
	/* border:1px solid #000; */
	width: 100%;
	height: 80upx;
	margin-left: 20upx;
	margin-top: 30upx;
}
.toptext1{
	font-size:20upx;
	font-weight:300;
	margin-left: 350upx;
	
}
.wlpxia1{
	font-size: 30upx;
	margin-left: 20upx;
	margin-top: 20upx;
}
.wlpxia2{
	font-weight:100;
	font-size: 20upx;
	margin-left: 20upx;
	margin-top: 20upx;
}
.top{
	width: 100%;
	/* border:1px solid #000; */
	height: 520upx;
}
.toptext5{
	font-size:20upx;
	font-weight:300;
	margin-left: 400upx;
}
.wlpxia5{
	font-weight:100;
	font-size: 20upx;
	margin-top: -20upx;
	
	
}
.top5{
	width: 100%;
	height: 20upx;
	/* border:1px solid #000; */
}
.bottom{
	width: 100%;
	/* border:1px solid #000; */
	height: 230upx;
	
}
.bottom image{
	width: 300upx;
	height: 200upx;
	margin: 20upx;
}
.ccc{
	margin-top: -150upx;
	margin-left: 320upx;
}
</style>
