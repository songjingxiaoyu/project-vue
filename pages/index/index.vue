<template>
	<view class="indexContainer">
        <!-- 头部区域 -->
		<view class="header">
		    <image src="../../static/images/logo.png" mode=""></image>
            <view class="search">
                <i class='iconfont icon-sousuo'></i>
                <input type="text" placeholder="搜索商品" placeholder-class="placeholder"/>
            </view>
            <button class="btn">登录</button>
		</view>
        <!-- 导航区域 -->
        <scroll-view enable-flex scroll-x="true" class="navScroll">
            <view class="navItem active">推荐</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
            <view class="navItem">商品</view>
        </scroll-view>
        <!-- 内容区域 -->
        <Recommend></Recommend>
	</view>
</template>

<script>
    import Recommend from '../../components/recommend/recommend.vue'
	export default {
		data() {
			return {
				
			}
		},
		components:{
            Recommend
        }
	}
</script>

<style lang="stylus">
.indexContainer
    // 头部区域
    .header
        display flex
        padding 10rpx 0
        image
            width 140rpx
            height 60rpx
            margin 10rpx 20rpx
        .search
            position relative
            width 420rpx
            height 60rpx
            background #ededed
            .iconfont
                font-size 30rpx
                position absolute
                top 25%
                left 10rpx
            input
                widows 380rpx
                height 60rpx
                margin-left 50rpx
            .placeholder
                font-size 26rpx
                text-align center
        .btn
            width 110rpx
            height 60rpx
            border-radius 4rpx
            padding 0 4rpx
            font-size 24rpx
            text-align center
            line-height 60rpx
            color #BB2C08
    // 导航区域
    .navScroll
        white-space nowrap
        width 100%
        height 80rpx
        .navItem
            position relative
            display inline-block
            width 140rpx
            height 80rpx
            text-align center
            line-height 80rpx
            font-size 28rpx
            &.active:after
                content ''
                position absolute
                bottom 0
                left 0
                height 1rpx
                width 100%
                background #BB2C08
                
</style>
