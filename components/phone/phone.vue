<template>
	<view class="phoneContainer">
		<view class="logo">
		    <image src="../../static/images/login/login-logo.png" mode=""></image>
		</view>
        <view class="phone">
            <input class="phoneInput" type="text" value="" placeholder="请输入手机号" placeholder-class="phonePlaceholder"/>
            <view class="password">
                <input class="passwordInput" type="password" value=""  placeholder="请输入短信验证码" placeholder-class="passwordPlaceholder"/>
                <view class="get">
                    获取验证码
                </view>
            </view>
            <view class="question">
                <text class="meet">遇到问题？</text>
                <text class="usePassword">使用密码验证登录</text>
            </view>
            <view class="login">
                <text>登录</text>
            </view>
            <view class="agree">
                <image src="../../static/images/login/agree.png" mode=""></image>
                <text>我同意《服务条款》和《网易隐私政策》</text>
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
            .get
                position absolute
                right 60rpx
                bottom 10rpx
                width 164rpx
                height 54rpx
                border 1rpx solid #eee
                text-align center
                line-height 54rpx
        .question
            height 80rpx
            margin-left 30rpx
            line-height 80rpx
            .meet
                margin 30rpx
                color #888
                font-size 24rpx
            .usePassword
                margin-left 230rpx
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
        .agree
            margin-left 40rpx
            margin-top 30rpx
            image
                width 34rpx
                height 34rpx
            text
                font-size 26rpx
        .other
            margin-left 300rpx
            margin-top 70rpx
            
</style>
