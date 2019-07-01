<template>
	<view class="content">

		<text class="weatherTitle">气候条件</text>
		<view class="detailWeather">
			<view class="humidity">
				<!-- 潮湿度 -->
			</view>
			<view class="airPressure">
				<!-- 气压 -->
			</view>
			<view class="visibility">
				<!-- 可见度 -->
			</view>
		</view>
		<text class="sunTitle">日光指数</text>
		<view class="sunSituation">
			<view class="sunWear">
				<!-- 穿衣指数 -->
			</view>
			<view class="sunLevel">
				<!-- 紫外线强度 -->
			</view>
			<view class="sunWash">
				<!-- 洗衣指数 -->
			</view>
		</view>
		<text class="windTitle">风条件</text>
		<view class="windSituation">

			<view class="windDirection">
				<!-- 风向 -->
			</view>
			<view class="windSpeed">
				<!-- 风速 -->
			</view>
			<view class="airCondition">
				<!-- 空气指数 -->
			</view>
		</view>
		<button class="back" type="default">➭</button>
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
	page{
		background: linear-gradient(to bottom right, #44FCA9, #44FCEA);
	}
	.content {
		text-align: left;
		font-size: 40upx;
		color: white;
	}

	/* 气候条件 */
	.detailWeather {
		height: 300upx;
	}

	.detailWeather view {
		display: inline-block;
		border: 1upx solid white;
	}

	.humidity {
		height: 300upx;
		width: 30%;
	}

	.airPressure {
		height: 300upx;
		width: 30%;
	}

	.visibility {
		height: 300upx;
		width: 30%;
	}

	/* 日光条件 */
	.sunSituation {
		height: 300upx;
	}

	.sunSituation view {
		display: inline-block;
		border: 1upx solid white;
	}

	.sunWear {
		height: 300upx;
		width: 30%;
	}

	.sunWash {
		height: 300upx;
		width: 30%;
	}

	.sunLevel {
		height: 300upx;
		width: 30%;
	}

	/* 风条件 */
	.windSituation {
		height: 300upx;
	}

	.windSituation view {
		display: inline-block;
		border: 1upx solid white;
	}

	.windDirection {
		height: 300upx;
		width: 30%;
	}

	.windSpeed {
		height: 300upx;
		width: 30%;
	}

	.airCondition {
		height: 300upx;
		width: 30%;
	}
	/* 返回按钮 */
	.back{
		margin-top: 10%;
		width: 40%;
		font-size: 60upx;
		background: none;
	}
</style>
