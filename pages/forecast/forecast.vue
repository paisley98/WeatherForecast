<template>
	<view class="content">
		<view class="title">
			<text class="maintitle">5天的预测</text>
		</view>
		<view class="fiveDays">
			<view class="today">
				<text class="todayWeather">{{firstweather}}</text>
			</view>
			<view class="secondDay">
				<text class="secondDayWeather">{{secondweather}}</text>
			</view>
			<view class="thirdDay">
				<text class="thirdDayWeather">{{thirdweather}}</text>
			</view>
			<view class="fourthDay">
				<text class="fourthDayWeather">{{fourthweather}}</text>
			</view>
			<view class="fifthDay">
				<text class="fifthDayWeather">{{fifthweather}}</text>
			</view>
		</view>
		<view class="todayAdvise">
			<text class="advise">{{advise}}</text>
		</view>
		<view class="back">
			<button class="backButton">⇦</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				firstweather:'晴',
				secondweather:'晴',
				thirdweather:'晴',
				fourthweather:'晴',
				fifthweather:'晴',
				advise:'今天有点凉哦！注意加衣服',
			}
		},
		methods: {

		}
	}
</script>

<style>
	page {
		background: linear-gradient(to bottom right, #44FCA9, #44FCEA);
	}

	.content {
		text-align: center;
		color: white;
	}

	.title {
		font-size: 40upx;
		height: 100upx;
		text-align: left;
	}
	.maintitle{
		position: relative;
		top: 30upx;
	}
	/* 五天的天气 */
	.fiveDays view {
		display: inline-block;
		border: 5upx solid white;
		margin: 8upx;
		width: 15%;
		height: 800upx;
	}
	.todayAdvise {
		font-size: 40upx;
		margin-top: 10%;
	}

	.backButton {
		margin-top: 10%;
		width: 40%;
		font-size: 60upx;
		background: none;
	}
</style>
