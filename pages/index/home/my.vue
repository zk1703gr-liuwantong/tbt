<!-- html部分 -->
<template>
	<div id="app">
		<view class="div1">
			<view class="dengru">
				<view class="yuan" @click="fn">
					<image src="../../../static/imgs/zjs.png"></image>
				</view>
				<!-- <view class="zimu" @click="fn" v-show="true">
					<h2>登录土巴兔</h2>
				</view> -->
				<view class="zimu" >
					<h2>{{cname}}</h2>
				</view>
				<view class="tubi" @click="fn">
					<text>领取兔币</text>
				</view>
				<view class="fanutop">
					<view class="fabu">
						<text class="o">0</text><br/>
						<text>发布</text>
					</view>
					<view class="fabu">
						<text class="o">0</text><br/>
						<text>收藏</text>
					</view>
					<view class="fabu">
						<text class="o">0</text><br/>
						<text>关注</text>
					</view>
					<view class="fabu">
						<text class="o">0</text><br/>
						<text>粉丝</text>
					</view>
				</view>
			</view>
		</view>
		<view class="div2">
			<text class="div2ziti">我的家</text>
			<button class="button1">立即享受专属服务</button>
			<view class="div2ziti2">
				<text>预约量房</text>
				<text>/</text>
				<text>免费设计</text>
				<text>/</text>
				<text>报价装修</text>
			</view>
		</view>
		<view class="div4">
			<text class="div3ziti">常用工具</text>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			
		</view>
		<view class="div4">
			<text class="div3ziti">第三方服务</text>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			<view class="xiaodiv2">
				<image src="../../../static/imgs/001.jpg"></image><br>
				<text>全屋定制</text>
			</view>
			
		</view>
	</div>
</template>
<!-- js部分 -->
<script>
	export default {
		name:'',
		data() {
			return {
				cname:'',
				flag:false
			};
		},
		methods:{
			fn(){
				// uni.navigateTo({
				// 	url:"login"
				// });
				if(this.cname==''){
					uni.switchTab({
						url:"login"
					})
				}else{
					uni.switchTab({
						url:"index"
					})
				}
				
				console.log("aaa")
			},
			
		},
		mounted(){
		var userid;
		uni.getStorage({
			key:'baseUser',
			success: (res) => {
				this.cname=res.data.cname
			}
		})
	}
	}
</script>
<!-- css部分 -->
<style>
	.yuan image{
		border-radius: 75upx;
		width: 150upx;
		height: 150upx;
		margin: 25upx;
	}
	.dengru{
		width: 100%;
		height: 350upx;
		/* border:1px solid #000; */
		/* background: #FFF; */
	}
	.zimu{
		/* border:1px solid #000; */
		width: 200upx;
		height: 50upx;
		margin-left: 200upx;
		margin-top: -125upx;
	}
	.tubi{
		width: 150upx;
		height: 50upx;
		/* border:1px solid #000; */
		margin-left: 550upx;
		font-size: 25upx;
		margin-top: -35upx;
		/* margin-left: 20upx; */
	}
	.o{
		display: inline-block;
		
	}
	.fabu{
	float: left;
	width: 100upx;
	height: 100upx;
	/* border:1px solid #000; */
	text-align: center;
	margin-left: 65upx;
	
	
	}
	.fanutop{
		margin-top: 80upx;
		height: 150upx;
		width: 100%;
	}
	.div1{
		width: 100%;
		background:#CCCCCC;
		height: 100%;
	}
	.div2ziti{
		font-size: 40upx;
		font-weight:bold;
		margin: 50upx;
		margin-top: 50upx;
	}
	.button1{
		border-radius: 60upx;
		height: 90upx;
		background: #2E8B57;
		width: 300upx;
		text-align: center;
	}
	.div2ziti2{
		width: 100%;
		height: 50upx;
		/* border:1px solid #000; */
		text-align: center;
		margin-top: 20upx;
	}
	.div2ziti2 text{
		margin-left: 20upx;
		font-size: 35upx;
	}
	.div2{
		width: 100%;
		height: 250upx;
		/* border:1px solid #000; */
	}
	.xiaodiv{
		/* border:1px solid #000; */
		width: 120upx;
		height: 100upx;
		float: left;
		margin-left: 50upx;
		margin-top: 80upx;
		text-align: center;
	}
	.xiaodiv2{
		/* border:1px solid #000; */
		width: 120upx;
		height: 100upx;
		float: left;
		margin-left: 50upx;
		margin-top: 80upx;
		text-align: center;
	}
	.xiaodiv image{
		width: 120upx;
		height: 100upx;
	}
	.xiaodiv2 image{
		width: 120upx;
		height: 100upx;
	}
	.xiaodiv text{
		font-size: 25upx;
		margin-left: 10up;
		
	}
	.xiaodiv2 text{
		font-size: 25upx;
		
	}
	.div3ziti{
		font-size: 40upx;
		font-weight:bold;
		/* margin: 50upx; */
		/* margin-top: 50upx; */
		margin-left: -620upx;
		margin-top: 10upx;
	}
	.div4{
		width: 100%;
		height: 430upx;
		/* border:1px solid #000 */
		margin-top: 20upx;
	}
	
</style>
