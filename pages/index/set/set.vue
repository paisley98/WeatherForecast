<template>
	<view class="content">
		<view class="settitle">
			<text class="title">设置</text>
		</view>
		<view class="local">
			<view class="broswer">
				<input type="text" class="search" height="20px" />
			</view>
			<view class="submit">
				<button type="default" class="button">搜索</button>
			</view>
		</view>
		<text class="titletheme">选择你喜欢的主题</text>
		<view class="theme">
			<view class="red"></view>
			<view class="blue"></view>
			<view class="green"></view>
			<view class="yellow"></view>
		</view>
		<button class="allsubmit">完成</button>
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
	page {
		background: linear-gradient(to bottom right, #44FCA9, #44FCEA);
		color: #FFFFFF;
	}

	.settitle {
		height: 10%;
	}

	.title {
		font-size: 50%;
		position: relative;
		top: -10upx;

	}

	.button {
		width: 40upx;
		position: absolute;
		left: 70%;
		margin: 5upx;
		background: none;
		color: white;
	}

	.broswer {
		display: flex;
		align-items: center;
		height: 30upx;
		border-radius: 5px;
		border: 2upx solid white;
		width: 90%;
		margin-left: 5%;
	}

	.search {
		flex: 1;
		font-size: 15upx;
	}

	.titletheme {
		font-size: 10upx;
	}

	.theme view {
		border: 1px solid white;
		padding: 10upx;
		margin: 10upx;
		border-radius: 25upx;
	}

	.red {
		background: linear-gradient(to right, #FC5190, #FFC4E2);
	}

	.blue {
		background: linear-gradient(to right, #70B0FF, #93E9FA);
	}

	.green {
		background: linear-gradient(to right, #85FF75, #44FCEA);
	}

	.yellow {
		background: linear-gradient(to right, #FFFD6E, #FFFED4);
	}

	.allsubmit {
		position: absolute;
		top: 80%;
		width: 90%;
		margin: 5%;
		background: none;
		color: white;
	}
</style>
