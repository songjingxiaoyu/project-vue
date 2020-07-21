<template>
	<view class="phoneContainer">
		<view class="logo">
		    <image src="../../static/images/login/login-logo.png" mode=""></image>
		</view>
        <view class="phone">
            <input class="phoneInput" type="text" value="" placeholder="邮箱账号" placeholder-class="phonePlaceholder"/>
            <view class="password">
                <input class="passwordInput" type="password" value=""  placeholder="密码" placeholder-class="passwordPlaceholder"/>
            </view>
            <view class="question">
                <text class="meet">注册账号</text>
                <text class="usePassword">忘记密码</text>
            </view>
            <view class="login">
                <text>登录</text>
            </view>
            
            <view class="other">
                其他登录方式>
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
.phoneContainer
    .logo
        image
            width 268rpx
            height 90rpx
            margin-top 70rpx
            margin-left 260rpx
    .phone
        
        .phoneInput
            margin-left 30rpx
            width 670rpx
            height 90rpx
            border-bottom 1rpx solid #eee
        .phonePlaceholder
            margin-left 20rpx
        .password
            position relative
            .passwordInput
                margin-left 30rpx
                width 670rpx
                height 90rpx
                border-bottom 1rpx solid #eee
            .passwordPlaceholder
                margin-left 20rpx
        .question
            height 80rpx
            margin-left 30rpx
            line-height 80rpx
            .meet
                margin 30rpx
                color #888
                font-size 24rpx
            .usePassword
                margin-left 400rpx
                color #888
                font-size 24rpx
        .login
            width 670rpx
            height 94rpx
            background #BB2C08
            border-radius 10rpx
            margin-left 40rpx
            text
                color #fff
                font-size 30rpx
                margin-left 300rpx
                line-height 94rpx
        .other
            margin-left 300rpx
            margin-top 70rpx
            
</style>
