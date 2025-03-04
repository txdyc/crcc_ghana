<template>
	<view class="content">
		<swiper class="swiper" :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000" circular>
			<swiper-item>
				<view class="swiper-item">aaa</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">bbb</view>
			</swiper-item>
		</swiper>
		<swiper class="notice" :autoplay="true" :interval="2000" :duration="1000" vertical circular>
			<swiper-item>
				<view class="swiper-item">通知1</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">通知2</view>
			</swiper-item>
		</swiper>
		<uni-section title="新闻" type="line">
			<uni-collapse  accordion v-model="accordionVal" @change="change">
				<uni-collapse-item title="时政">
					<view class="mycontent">
						<text class="text">手风琴效果同时只会保留一个组件的打开状态，其余组件会自动关闭。</text>
					</view>
				</uni-collapse-item>
				<uni-collapse-item title="经济">
					<view class="mycontent">
						<text class="text">手风琴效果同时只会保留一个组件的打开状态，其余组件会自动关闭。</text>
					</view>
				</uni-collapse-item>
				<uni-collapse-item title="娱乐">
					<view class="mycontent">
						<text class="text">手风琴效果同时只会保留一个组件的打开状态，其余组件会自动关闭。</text>
					</view>
				</uni-collapse-item>
			</uni-collapse>
		</uni-section>
	</view>
</template>

<script setup>

</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		
		.swiper {
			width: 100vw;
			height: 300rpx;
			
			.swiper-item {
				width: 100%;
				height: 100%;
			}
		}
		
		.notice {
			margin-top: 4rpx;
			width: 100vw;
			height: 40rpx;
		}
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	
	.mycontent {
		padding: 15px;
	}
	
	.text {
			font-size: 14px;
			color: #666;
			line-height: 20px;
		}
</style>
