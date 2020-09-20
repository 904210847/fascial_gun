<template>
	<view>
		<view class="">
			<view class="cu-item shadow">
				<view class="image">
					<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg" mode="widthFix"></image>
				</view>
			</view>
		</view>
		<view>
			<van-divider contentPosition="center" customStyle="color: black; border-color: #1989fa; font-size: 18px;">
				请选择放松的类型
			</van-divider>
		</view>
		<!-- <view>
			<view class="cu-card case" :class="isCard?'no-card':''">
				<view class="cu-item shadow">
					<view class="image">
						<image src="https://ossweb-img.qq.com/images/lol/web201310/skin/big10006.jpg"
						 mode="widthFix"></image>
						<view class="cu-tag bg-blue">史诗</view>
						<view class="cu-bar bg-shadeBottom">
							<text class="text-cut">我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。</text>
						</view>
					</view>
					<view class="cu-list menu-avatar">
						<view class="cu-item">
							<view class="content flex-sub">
								<view class="text-grey">运动放松方案</view>
								<view class="text-gray text-sm flex justify-between">
									跑步、篮球、游泳
									<view class="text-gray text-sm">
										<text class="lg text-gray" class="cuIcon-right"></text>
									</view>
								</view>
							</view>
						</view>
					</view>
				</view>
			</view>
		</view> -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			console.log("显示index的页面");
			const bgAudioMannager = uni.getBackgroundAudioManager();
			bgAudioMannager.title = '致爱丽丝';
			bgAudioMannager.singer = '暂无';
			bgAudioMannager.coverImgUrl = 'https://img-cdn-qiniu.dcloud.net.cn/uniapp/audio/music.jpg';
			bgAudioMannager.src = 'https://img-cdn-qiniu.dcloud.net.cn/uniapp/audio/music.mp3';
		},
		methods: {

		}
	}
</script>

<style>
	/**
	 * 设置图片的样式
	 */
	image{
		
	}
</style>
