<template>
	<view class="content">
		<view class="place">
			<text>{{place}}</text>
		</view>

		<view class="message">
			<view class="todayMes">

				<view class="todayWeathertext">
					<text class="todayWeather"> {{weather}}</text>
				</view>

				<view class="todayWeatherImage">
					<image v-bind:src="address" class="todayWeatherImg" id="Wimage"></image>
				</view>

			</view>
			<view class="temperature">
				<view class="temperatureWord">
					<text class="temperatureText">{{temperature}}</text>
				</view>
			</view>
		</view>

		<view class="navigate">
			<view class="left">
				<button type="default" class="leftbut">⇦</button>
			</view>
			<view class="right">
				<button type="default" class="rightbut">⇨</button>
			</view>
		</view>
		<view class="setter">
			<button type="default" class="set">设置</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				place: '北京',
				address: '/static/cloud.rain.png',
				weather: '雨',
				temperature: '17℃',
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	page {
		background: linear-gradient(to bottom right, #44FCA9, #44FCEA);
	}

	uni-page-body {
		background: none;
	}

	.content {
		color: white;
		font-size: 100upx;
	}

	.place {
		text-align: left;
	}

	.message {
		text-align: center;
		margin-top: 30%;
	}

	.todayMes view {
		display: inline;

	}

	.todayWeathertext {
		font-size: 200upx;

	}

	.todayWeatherImg {
		height: 200upx;
		width: 200upx;
		animation: myfirst 5s infinite;
		-webkit-animation: myfirst 7s infinite;
		position: relative;
		top: 20px;
	}

	@keyframes myfirst {
		from {
			opacity: 1.0;
		}

		50% {
			opacity: 0.2;
		}

		to {
			opacity: 1.0;
		}
	}

	@-webkit-keyframes myfirst {
		from {
			opacity: 1.0;
		}

		50% {
			opacity: 0.2;
		}

		to {
			opacity: 1.0;
		}
	}

	.temperatureWord {
		font-size: 150upx;
	}

	.navigate view {
		display: inline-block;
		margin-top: 20%;
	}

	.left {
		width: 50%;
	}

	.leftbut {
		width: 40%;
		position: relative;
		left: -40upx;
		background: none;
		color: white;
		font-size: 50upx;
	}

	.right {
		width: 50%;
	}

	.rightbut {
		width: 40%;
		position: relative;
		right: -40upx;
		background: none;
		color: white;
		font-size: 50upx;
	}

	.setter {
		position: fixed;
		left: 0;
		bottom: 2%;
		right: 0;
	}

	.set {
		width: 20%;
		border-radius: 25px;
		color: #FFFFFF;
		background-color: #94F76C;
	}
</style>
