<!-- html部分 -->
<template>
	<div id="app">
		<view>
			<mSearch></mSearch>
		</view>
		<view>
			<wlp></wlp>
		</view>
		<view class="div3">
			<view class="dadada">
				<view class="xiaotu">
					<image src="../../../static/imgs/001.jpg"></image>
				</view>
				<view class="zitidiv">
					<text class="ziti">算报价</text>
				</view>
			</view>
			<view class="dadada">
				<view class="xiaotu">
					<image src="../../../static/imgs/002.jpg"></image>
				</view>
				<view class="zitidiv">
					<text class="ziti">找设计</text>
				</view>
			</view>
			<view class="dadada">
				<view class="xiaotu">
					<image src="../../../static/imgs/003.jpg"></image>
				</view>
				<view class="zitidiv">
					<text class="ziti">黑卡会员</text>
				</view>
			</view>
			<view class="dadada">
				<view class="xiaotu">
					<image src="../../../static/imgs/004.jpg"></image>
				</view>
				<view class="zitidiv">
					<text class="ziti">装修分期</text>
				</view>
			</view>
		</view>
		<view class="div4">
			<view class="sq">
				<image src="../../../static/imgs/5.jpg"></image>
			</view>
			<view class="sq2">
				<image src="../../../static/imgs/3.jpg"></image>
			</view>
			<view class="sq3">
				<image src="../../../static/imgs/4.jpg"></image>
			</view>
		</view>
		<view>
			<demo></demo>
		</view>
		
	</div>
</template>
<!-- js部分 -->
<script>
	import demo from "@/components/demo/demo.vue";
	 import mSearch from '@/components/mehaotian-search/mehaotian-search.vue';
	 import wlp from '@/components/wlp-swiper-banner/wlp-swiper-banner.vue';
	 
	export default {
		components:{mSearch,wlp,demo},
		name:'',
		data() {
			return {
				
			};
		},
		methods:{
			
		},mounted(){
			console.log("aaaaaaaaaaaaaaaaaaa")
		}
	}
</script>
<!-- css部分 -->
<style>
.xiaotu image{
	width: 120upx;
	height: 100upx;
	float: left;
	
}
.xiaotu{
	margin-left: 30upx;
	width: 120upx;
	height: 100upx;
	/* border:1px solid #000; */
	float: left;
	margin-top: 30upx;
}
.ziti{
	font-size: 15upx;
	margin-top: 100upx;
	margin-left: 10upx;
	
}
.zitidiv{
	height: 30upx;
	width: 60upx;
	/* border:1px solid #000; */
	margin-left: 55upx;
	float: left;
	/* margin-top: 10upx; */
	
	
}
.div3{
	width: 100%;
	height: 190upx;
	/* background: #CCCCCC; */
	
	
}
.dadada{
	width: 150upx;
	height: 150upx;
	float: left;
	margin-left: 30upx;
}
.div4{
	/* border:1px solid #000; */
	width: 100%;
	height: 400upx;
}
.sq image{
	width: 50%;
	height: 350upx;
	float: left;
}
.sq2 image{
	width: 50%;
	height: 175upx;
	float: left;
	
}
.sq3 image{
	width: 50%;
	height: 175upx;
	float: left;
}
</style>
