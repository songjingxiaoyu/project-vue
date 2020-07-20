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
    .header
        margin-left 10rpx
    .content
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
                height 220rpx
                width 100%
                background white
                .goodsImg
                    width 172rpx
                    height 172rpx
                .detail
                    .name
                        font-size 26rpx
                    .des
                        font-size 24rpx
                    .price
                        font-size 26rpx
                .count
                    width 180rpx
                    height 60rpx
                    border 1rpx solid #d9d9d9
                    .number
                        border-left 1rpx solid #d9d9d9
                        border-right 1rpx solid #d9d9d9
            .order
                position absolute
                bottom 0
                right 0
                background white
                width 100%
                height 750rpx
                .btn
                    width 225rpx
                    height 118rpx
                    background #BB2C08
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
