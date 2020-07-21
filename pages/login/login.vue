<template>
	<view class="loginContainer">
        <!-- logo区域 -->
		<view class="logo">
		    <image src="../../static/images/login/login-logo.png" mode=""></image>
		</view>
        <!-- 手机/邮箱登录 -->
        <view class="phoneMail">
            <view class="phone">
                <image src="../../static/images/login/手机.png" mode=""></image>
                <text>手机号快捷登录</text>
            </view>
            <view class="mail">
                <image src="../../static/images/login/邮箱.png" mode=""></image>
                <text>邮箱账号登录</text>
            </view>
        </view>
        <!-- 其他登录区域 -->
        <view class="other">
            <view class="otherItem weixin">
                <image src="../../static/images/login/微信.png" mode=""></image>
                <text>微信</text>
            </view>
            <view class="borderLeft">
                
            </view>
            <view class="otherItem qq">
                <image src="../../static/images/login/qq.png" mode=""></image>
                <text>QQ</text>
            </view>
            <view class="borderRight">
                
            </view>
            <view class="otherItem weibo">
                <image src="../../static/images/login/微博.png" mode=""></image>
                <text>微博</text>
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
.loginContainer
    // logo区域
    .logo
        width 750rpx
        height 480rpx
        position relative
        image
            position absolute
            left 0
            top 0
            right 0
            bottom 0
            margin auto 
            width 268rpx
            height 90rpx
    // 手机/邮箱登录
    .phoneMail
        .phone
            color #fff
            background #BB2C08
        .mail
            color #BB2C08
        view
            position relative
            width 670rpx
            height 94rpx
            margin-bottom 32rpx
            margin-left 40rpx
            text-align center
            line-height 94rpx
            border 1rpx solid #BB2C08
            image
                position absolute
                left 185rpx
                top 30rpx 
                width 40rpx
                height 40rpx
    // 其他登录区域
    .other
        position fixed
        bottom 100rpx
        left 0
        width 750rpx
        height 40rpx
        display flex
        .weixin
            margin-right 30rpx
            margin-left 200rpx
        .borderLeft,.borderRight
            width 2rpx
            height 40rpx
            background #7F7F7F
        .qq
            margin 0 30rpx
        .weibo
            margin-left 30rpx
        .otherItem
            image
                width 40rpx
                height 40rpx
            text
                color #7F7F7F
</style>
