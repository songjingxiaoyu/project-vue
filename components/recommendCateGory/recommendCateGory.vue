<template>
	<view class="recommendCateGoryContainer">
		<image class="bigImg" src="../../static/images/logo.png" mode=""></image>
        <scroll-view enable-flex scroll-x="true" class="scrollContaoner">
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem">
                <image class="simImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <view>商品</view>
            </view>
            <view class="scrollItem more">
                查看更多>
            </view>
        </scroll-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="stylus">
.recommendCateGoryContainer
    .bigImg
        width 100%
        height 370rpx
    .scrollContaoner
        width 100%
        white-space nowrap
        .scrollItem
            width 200rpx
            display inline-block
            margin 20rpx 10rpx
            vertical-align top
            &.more
                height 200rpx
                font-size 26rpx
                background #eee
                text-align center
                line-height 200rpx
            image
                width 200rpx
                height 200rpx
                border-radius 10rpx
                background #eee
            view
                font-size 24rpx
                white-space pre-wrap
                text-align center
                
</style>
