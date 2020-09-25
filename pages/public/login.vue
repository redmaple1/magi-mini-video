<template>
	<view class="container">
		<view class="input-content">
			<view class="input-item">
				<text class="tit">账号</text>
				<input type="text" placeholder="请输入账号" />
			</view>
		</view>
	</view>
</template>

<script>
</script>

<style lang='scss'>
	.container {
		padding-top: 115px;
		position: relative;
		width: 100vw;
		height: 100vh;
		overflow: hidden;
		background: #fff;
	}
	
	.input-content{
		padding: 0 60upx;
	}

	.input-item {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		padding: 0 30upx;
		border: 1upx solid;
		border-radius: 15upx;
		border-color: $uni-border-color;
		height: 100upx;
		.tit{
			height: 80upx;
			line-height: 100upx;
			font-size: $font-base;
		}
	}
</style>
