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
				<navigator url="">←</navigator>
			</view>
			<view class="right">
				<navigator url="">→</navigator>
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
		font-size: 50%;
	}

	.place {
		text-align: center;
	}

	.message {
		text-align: center;
		margin-top: 30%;
	}

	.todayMes view {
		display: inline;

	}

	.todayWeathertext {
		font-size: 250%;

	}

	.todayWeatherImg {
		height: 100px;
		width: 100px;
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
		font-size: 250%;
	}

	.navigate view {
		display: inline-block;
		margin-top: 30%;
	}

	.left {
		width: 40%;
		margin-left: 5%;
		font-size: 150%;
	}

	.right {
		width: 50%;
		text-align: right;
		font-size: 150%;
	}

	.setter {
		position: fixed;
		left: 0;
		bottom: 2%;
		right: 0;
	}

	.set {
		width: 40%;
		border-radius: 25px;
		color: #FFFFFF;
		background-color: #94F76C;
	}
</style>
