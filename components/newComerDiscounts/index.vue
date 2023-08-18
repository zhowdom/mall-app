<template>
	<view class="newComerDiscounts-box boxsz">
		<view class="newComer-title flex alient-item-c justify-item-c">
			<view class="left">新人现时优惠</view>
			<view class="midle flex1">9.99元起</view>
			<text class="more">More ></text>
		</view>
	</view>
</template>

<script>
	export default {
		data () {
			return {
				
			}
		}
	}
</script>

<style lang="scss">
	.newComerDiscounts-box{
		width: 702rpx;
		height: 840rpx;
		background: linear-gradient(180deg, #FF9822 0%, #FFBD52 100%);
		border-radius: 16rpx;
		margin: 24rpx auto 0 auto;
		padding: 16rpx;
		.newComer-title{
			color: #fff;
			padding-top: 16rpx;
			.left{
				font-size: 40rpx;
				font-weight: 600;
				text-shadow: 0px 2px 4px #F86509;
				padding-right: 16rpx;
			}
			.midle{
				font-size: 32rpx;
				font-weight: 400;
				padding-left: 16rpx;
				border-left: 1rpx solid rgba(255,255,255,.3);
			}
			.more{
				font-size: 28rpx;
				font-weight: 500;
			}
		}
	}
</style>