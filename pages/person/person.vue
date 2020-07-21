<template>
	<view class="personContainer">
        <!-- 头部 -->
		<view class="header">
		    <image class="user" src="../../static/images/personal/personal.png" mode=""></image>
            <view class="text">
                <view>未登录</view>
                <view>点击登录账号</view>
            </view>
		</view>
        <!-- 资产 -->
        <view class="data">
            <view class="money">我的资产</view>
            <view class="list">
                <view class="listItem gold">
                    <view >￥0</view>
                    <view >回馈金</view>
                </view>
                <view class="listItem redPaper">
                    <view >0</view>
                    <view >红包</view>
                </view>
                <view class="listItem coupon">
                    <view >0</view>
                    <view >优惠券</view>
                </view>
                <view class="listItem benefit">
                    <view >￥0</view>
                    <view >津贴</view>
                </view>
                <view class="listItem card">
                    <view >0</view>
                    <view >礼品卡</view>
                </view>
            </view>
        </view>
        <view class="dataNext">
            
        </view>
        <!-- 列表 -->
        <view class="menu">
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/订单.png" mode=""></image>
                    <view class="">我的订单</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/日历6.png" mode=""></image>
                    <view class="">周六一起拼</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/退货售后.png" mode=""></image>
                    <view class="">售后服务</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/邀请好友.png" mode=""></image>
                    <view class="">邀请返利</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/购物袋3-01.png" mode=""></image>
                    <view class="">优先购</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/钱.png" mode=""></image>
                    <view class="">积分中心</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/会员.png" mode=""></image>
                    <view class="">会员俱乐部</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/收货地址.png" mode=""></image>
                    <view class="">地址管理</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/售后无忧.png" mode=""></image>
                    <view class="">账号安全</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem">
                    <image src="../../static/images/personal/客服.png" mode=""></image>
                    <view class="">帮助与客服</view>
                </view>
            </view>
            <view class="menuContainer">
                <view class="menuItem last">
                    <image src="../../static/images/personal/反馈.png" mode=""></image>
                    <view class="">意见反馈</view>
                </view>
            </view>
        </view>
        <view class="menuNext">
            
        </view>
        <!-- 退出登录 -->
        <view class="quit">
            <view class="btn">
                退出登录
            </view>
        </view>
        <view class="quitNext">
            
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
.personContainer
    height 100vh
    width 100vh
    background #eee
    .header
        position relative
        height 268rpx
        width 100%
        background #F4CA7F
        display flex
        .user
            position absolute
            left 30rpx
            top 63rpx
            width 142rpx
            height 142rpx
            border-radius 50%
            background #fff
        .text
            position absolute
            left 200rpx
            top 95rpx
    .data
        height 285rpx
        width 100%
        background #fff
        .money
            width 100%
            height 105rpx
            border-bottom 1rpx solid #eee
            line-height 105rpx
            margin-left 30rpx
        .list
            height 180rpx
            display flex
            position relative
            .listItem
                font-size 24rpx
                height 180rpx
                width 13.5%
                text-align center
                margin-top 50rpx
    .dataNext
        height 20rpx
        background #eee
    .menu
        height 723rpx
        width 750rpx
        background #fff
        .menuContainer
            height 180rpx
            width 248rpx
            float left
            border-right 1rpx solid #eee
            border-bottom 1rpx solid #eee
            text-align center
            .menuItem
                margin-top 30rpx
                image
                    width 50rpx
                    height 50rpx
    .menuNext
        height 40rpx
        background #eee
    .quit
        height 96rpx
        width 100%
        background #fff
        border 1rpx solid #eee
        .btn
            line-height 96rpx
            margin-left 320rpx
    .quitNext
        height 20rpx
        background #eee
</style>
