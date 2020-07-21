<template>
	<view class="carContainer">
		<view class="header">
		    购物车
		</view>
        <view class="content">
            <!-- 未登录 -->
            <!-- <view class="noLogin">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <button class="btn">登录</button>
            </view> -->
            <!-- 已登录有商品 -->
            <view class="loginGoods">
                <view class="goods">
                    <view class='iconfont icon-xuanzhong '></view>
                    <image class="goodsImg" src="../../static/images/carts/emptyCart.gif" mode=""></image>
                    <view class="detail">
                        <view class="name">商品名称</view>
                        <view class="des">商品描述</view>
                        <view class="price">￥160</view>
                    </view>
                    <view class="count">
                        <view class="reduce">-</view>
                        <view class="number">2</view>
                        <view class="add">+</view>
                    </view>
                </view>
                <view class="order">
                    <view class='iconfont icon-xuanzhong '>已选 2</view>
                    <view class="allPrice">合计 ￥ 1100</view>
                    <button class="btn">下单</button>
                </view>
            </view>
            <!-- 已登录无商品 -->
            <!-- <view class="loginNoGoods">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <button class="btn">去购物吧</button>
            </view> -->
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
.carContainer
    background #eee
    height 100vh
    .header
        margin-left 10rpx
    .content
        height 100%
        // 未登录
        .noLogin
            margin-top 40%
            image
                margin-left 30%
                width 248rpx
                height 248rpx
            .btn
                width 480rpx
                height 92rpx
                background #BB2C08
        // 已登录有商品
        .loginGoods
            position relative
            .goods
                display flex
                position relative
                justify-content center
                height 220rpx
                width 100%
                background white
                .iconfont
                    position absolute
                    top 40%
                    left 40rpx
                    align-self center
                    width 38rpx
                    height 38rpx
                .goodsImg
                    position absolute
                    top 30rpx
                    left 100rpx
                    width 172rpx
                    height 172rpx
                .detail
                    position absolute
                    top 50rpx
                    left 320rpx
                    .name
                        font-size 26rpx
                        height 36rpx
                        margin-bottom 10rpx
                    .des
                        margin 0 0 30rpx 0
                        font-size 24rpx
                        height 36rpx
                    .price
                        font-size 26rpx
                        height 39rpx
                .count
                    position absolute
                    bottom 30rpx
                    right 20rpx
                    height 60rpx
                    display flex
                    justify-content center
                    view
                        width 60rpx
                        border 1rpx solid #d9d9d9
                        text-align center
                        line-height 60rpx
                    .reduce
                        border-right 0rpx solid #d9d9d9
                    .add
                        border-left 0rpx solid #d9d9d9
            .order
                position fixed
                left 0
                bottom 0rpx
                background white
                width 100%
                height 118rpx
                .iconfont
                    position absolute
                    top 30%
                    left 40rpx
                .allPrice
                    position absolute
                    top 30%
                    right 250rpx
                .btn
                    position absolute
                    top 0
                    right 0rpx
                    width 225rpx
                    height 118rpx
                    background #BB2C08
                    text-align center
                    line-height 118rpx
                    color white
                
        // 已登录无商品
        .loginNoGoods
            margin-top 40%
            image
                margin-left 30%
                width 248rpx
                height 248rpx
            .btn
                width 480rpx
                height 92rpx
                background #BB2C08
</style>
