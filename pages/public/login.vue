<template>
	<view class="login">
		<view class="content">
			<!-- 主体表单 -->
			<view class="main">
				<winput
				  type="text"
				  maxlength="11"
				  placeholder="用户名"
				></winput>
				<winput
				 type="password"
				 placeholder="密码"
				></winput>
			</view>
		</view>
	</view>
	</view>
</template>

<script>
	var _this;
	import winput from '../../components/watch-login/watch-input.vue'
	
	export default{
		data(){
			phoneData:''
		},
		components:{
			winput
		},
		mounted(){
			_this = this;
		}
	}
</script>

<style>
	@import url("../../components/watch-login/css/icon.css");
	@import url("./css/main.css");
</style>
