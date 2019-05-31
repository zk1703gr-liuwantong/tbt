<!-- html部分 -->
<template>
	<div id="app">
		<view class="divtop">
			<view class="logo">
				<image src="../../../static/imgs/rabbit.jpg"></image>
			</view>
			<view>
				<input  type="text" placeholder="请输入用户名" class="inp" v-model="username"/>
				<input type="password" placeholder="请输入密码" class="inp" v-model="password"/>
				<button class="button" @click="fn">登陆</button>
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
				username:"lhx",
				password:"123456"
			};
		},
		methods:{
			fn(){
				uni.request({
					url: this.url+"baseUser/login", //仅为示例，并非真实接口地址。
					data: {
						username:this.username,
						password:this.password
					},
					header: {
						'custom-header': 'hello' //自定义请求头信息
					},
					success: (res) => {
						console.log(res.data);
					}
				});
			}
		}
	}
</script>
<!-- css部分 -->
<style>
	.logo image{
		width: 300upx;
		height: 300upx;
	}
	.logo{
		text-align: center;
	}
	.inp{
		
		width: 80%;
		text-align: center;
		height: 80upx;
		margin-left: 10%;
		margin-top: 5upx;
		border-bottom:seagreen solid 0.9upx;
	}
	.button{
		width: 100%;
		height: 100upx;
		
		background: #FFF;
		margin-top: 5upx;
		text-align: center;
		
	}
	.divtop{
		margin-top: 35%;
	}
</style>
