<template>
	<view>
		<!-- 按钮 -->
		<button 
			:class="['buttonBorder',_rotate?'dlbutton':'dlbutton_loading']"
			:style="{'background':bgColor,'color':fontColor}"
			
			@click="$emit('click', $event)"
			@contact="$emit('contact', $event)"
			@error="$emit('error', $event)"
			@getphonenumber="$emit('getphonenumber', $event)"
			@getuserinfo="$emit('getuserinfo', $event)"
			@launchapp="$emit('launchapp', $event)"
			@longtap="$emit('longtap', $event)"
			@opensetting="$emit('opensetting', $event)"
			@touchcancel="$emit('touchcancel', $event)"
			@touchend="$emit('touchend', $event)"
			@touchmove="$emit('touchmove', $event)"
			@touchstart="$emit('touchstart', $event)"
		></button>
	</view>
</template>

<script>
	export default{
		props:{
			text: String, //显示文本
			rotate: {
				//是否启动加载
				type: [Boolean,String],
				default: false,
			},
			bgColor:{
				//按钮北京颜色
				type: String,
				default: "linear-gradient(to right, rgba(0,0,0,0.7), rgba(0,0,0,0.6))",
			},
			fontColor:{
				type: String,
				default: "#FFFFFF",
			}
		},
		computed:{
			_rotate(){
				return String(this.rotate) !== 'false'
			}
		}
	}
</script>

<style>
</style>
