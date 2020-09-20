<template>
	<view>
		<view class="own-img">
			<van-row>
				<van-col span="10" offset="8">
					<van-image round width="6rem" height="6rem" src="https://img.yzcdn.cn/vant/cat.jpeg"/><br>
				</van-col>
			</van-row>
			<van-row>
				<van-col offset="8" span="6">
					nickName
				</van-col>
				<van-col span="4">
					sex
				</van-col>
			</van-row>
		</view>
		<view>
			<van-cell title="我的信息" is-link />
			<van-cell title="放松恢复记录" is-link />
			<van-cell title="我的方案" is-link />
			<van-cell title="我的设备" is-link />
		</view>
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

<style>
	/**
	 * 自己定义的头像的样式
	 */
	.own-img{
		padding-bottom : 40px;
	}
</style>
