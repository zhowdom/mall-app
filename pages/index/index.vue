<template>
	<view class="indexBox">
		<uni-nav-bar color="#fff" :shadow="false" backgroundColor="#fd93c7" @clickLeft="onClickLeft" @clickTitle="onClickTitle" @clickRight="onClickRight" shadow statusBar shadow="false">
			<view slot="left" class="index-topheader-left flex flex1 alient-item-c justify-item-c">
				<image class="index-topheader-logo" src="../../static/index_logo.png"></image>
			</view>
			<view class="index-topheader-center flex alient-item-c justify-item-c">
				<image class="index-topheader-pic" src="../../static/index_search.png"></image>
				<image class="index-topheader-pic" src="../../static/index_favorite.png"></image>
				<image class="index-topheader-pic" src="../../static/index_message.png"></image>
			</view>
			<view slot="right" class="index-topheader-right flex alient-item-c justify-item-c">
				<image class="index-topheader-pic" src="../../static/index_customer.png"></image>
			</view>
		</uni-nav-bar>
		
		<!--新人限時優惠-->
		<newComerDiscounts />
	</view>
</template>

<script>
	import newComerDiscounts from '../../components/newComerDiscounts/index.vue'
	export default {
		components: {
			newComerDiscounts
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {},
		methods: {
			onClickLeft () {
				uni.showToast({
					title:'ok-ok',
					icon:'none'
				})
			},
			onClickTitle () {
				uni.showToast({
					title:'ok-ok',
					icon:'none'
				})
			},
			onClickRight () {
				uni.showToast({
					title:'ok-ok',
					icon:'none'
				})
			}
		}
	}
</script>

<style lang="scss">
	.indexBox{
		.index-topheader-center{
			display: flex;
			justify-items: end;
			margin-left:auto;
			.index-topheader-pic{
				margin-left:30rpx;
			}
		}
		.index-topheader-right{
			flex: 1;
			width: 320rpx;
		}
		.index-topheader-logo{
			width: 90rpx;
			height: 64rpx;
		}
		.index-topheader-pic{
			width:45rpx;
			height: 45rpx;
		}
	}
</style>
