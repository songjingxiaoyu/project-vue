<template>
	<view class="cateGoryContainer">
        <!-- 搜索区域 -->
		<view class="search">
            <i class='iconfont icon-sousuo'></i>
            <input type="text" placeholder="搜索商品" placeholder-class="placeholder"/>
		</view>
        <!-- 商品区域 -->
        <view class="content">
            <view class="left">
                <scroll-view scroll-y="true" class="leftScroll">
                    <view class="scrollItem active">商品</view>
                    <view class="scrollItem">商品</view>
                    <view class="scrollItem">商品</view>
                    <view class="scrollItem">商品</view>
                    <view class="scrollItem">商品</view>
                    <view class="scrollItem">商品</view>
                </scroll-view>
            </view>
            <view class="right">
                <scroll-view scroll-y="true" class="rightScroll">
                    <view class="list">
                        <image class="listImg" src="https://yanxuan.nosdn.127.net/13b5104f7b382c46afd827a9733075bf.jpg?quality=75&amp;type=webp&amp;imageView&amp;thumbnail=0x196"  mode=""></image>
                        <view class="listItem">
                            <image class="listItenImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                            <view class="text">列表商品</view>
                        </view>
                        <view class="listItem">
                            <image class="listItenImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                            <view class="text">列表商品</view>
                        </view>
                        <view class="listItem">
                            <image class="listItenImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                            <view class="text">列表商品</view>
                        </view>
                        <view class="listItem">
                            <image class="listItenImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                            <view class="text">列表商品</view>
                        </view>
                    </view>
                </scroll-view>
            </view>
        </view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="stylus">
.cateGoryContainer
    .search
        position relative
        padding 10rpx 0
        display flex
        justify-content center
        flex-flow row nowrap
        align-items center
        width 690rpx
        height 56rpx
        background #ededed
        align-items center
        border-radius 10rpx
        margin 10rpx auto
        .iconfont
            width 28rpx
            height 28rpx
        .placeholder
            text-align center
    .content
        display flex
        border-top 1rpx solid #d9d9d9
        height calc(100vh-76rpx)
        .left
            width 20%
            height 100%
            border-right 1rpx solid #d9d9d9
            .leftScroll
                .scrollItem
                    position relative
                    height 50rpx
                    margin-top 40rpx
                    text-align center
                    &.active:before
                        content ''
                        position absolute
                        left 0
                        top 0
                        border-left 3rpx solid #BB2C08
                        height 100%
                        margin-left 10rpx
        .right
            width 80%
            .rightScroll
                text-align center
                .list
                    margin 20rpx auto
                    width 528rpx
                    height 100%
                    .listImg
                        height 190rpx
                        width 528rpx
                    .listItem
                        display inline-block
                        width 33.33%
                       .listItenImg
                        width 144rpx
                        height 144rpx
                       .text
                        font-size 26rpx
</style>
