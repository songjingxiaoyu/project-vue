<template>
	<view class="recommendConyainer">
        <!-- 轮播图区域 -->
		<swiper class="banner" :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000">
		    <swiper-item>
		        <view class="swiper-item">
                    <img src="https://yanxuan.nosdn.127.net/e1d32c538a9fcf420411592746098ad2.jpg?type=webp&amp;imageView&amp;quality=75&amp;thumbnail=750x0">
                </view>
		    </swiper-item>
		    <swiper-item>
		        <view class="swiper-item">
                    <img src="https://yanxuan.nosdn.127.net/e4b5ab7f6bb4b286b9fe18e42bb1f731.jpg?type=webp&amp;imageView&amp;quality=75&amp;thumbnail=750x0">
                </view>
		    </swiper-item>
		    <swiper-item>
		        <view class="swiper-item">
                    <img src="https://yanxuan.nosdn.127.net/8104acf1cc1514a88ea0b7d030e9a55e.jpg?type=webp&amp;imageView&amp;quality=75&amp;thumbnail=750x0">
                </view>
		    </swiper-item>
            <swiper-item>
                <view class="swiper-item">
                    <img src="https://yanxuan.nosdn.127.net/99873ee03dbfa1fec94f273025baaf20.jpg?type=webp&amp;imageView&amp;quality=75&amp;thumbnail=750x0">
                </view>
            </swiper-item>
		</swiper>
        <!-- grow区域 -->
        <view class="grow">
            <view class="growItem">
                <image src="../../static/images/recommend/易.png" mode=""></image>
                <text>网易自营品牌</text>
            </view>
            <view class="growItem">
                <image src="../../static/images/recommend/售后无忧.png" mode=""></image>
                <text>30天无忧退货</text>
            </view>
            <view class="growItem">
                <image src="../../static/images/recommend/退款.png" mode=""></image>
                <text>48小时极速退款</text>
            </view>
        </view>
        <!-- 列表区域 -->
        <view class="list">
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
            <view class="listItem">
                <image src="../../static/images/carts/emptyCart.gif" mode=""></image>
                <text>居家生活</text>
            </view>
        </view>
        <!-- RecommendCateGory区域 -->
        <RecommendCateGory></RecommendCateGory>
	</view>
</template>

<script>
    import RecommendCateGory from '../../components/recommendCateGory/recommendCateGory.vue'
	export default {
		data() {
			return {
				
			};
		},
        components:{
            RecommendCateGory
        }
	}
</script>

<style lang="stylus">
.recommendConyainer
    .banner
        width 100%
        height 350rpx
        .swiper-item
            width 100%
            height 100%
            image
                width 100%
                height 100%
    .grow
        display flex
        white-space nowrap
        .growItem
            flex 1
            text-align center
            margin 10rpx 0
            image
                width 32rpx
                height 32rpx
                vertical-align middle
            text
                height 64rpx
                font-size 24rpx
    .list
        display flex
        flex-wrap wrap
        .listItem
            display flex
            width 20%
            flex-direction column
            align-items center
            image
                width 110rpx
                height 110rpx
                border-radius 10rpx
                
            text
                font-size 24rpx
                line-height 50rpx
                
</style>
