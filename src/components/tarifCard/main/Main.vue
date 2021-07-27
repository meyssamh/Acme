<template>
<div class="main">
	<!-- Background -->
	<app-background></app-background>
	<div class="main-container">
		<!-- Tarif logo -->
		<div class="play">
			<img class="img-play" src="../../../assets/play.png" alt="play">
		</div>
		<!-- Title -->
		<app-title :mainTitle="title"></app-title>
		<!-- Hints container -->
		<div class="text-container">
			<!-- First sign and text -->
			<div class="text">
				<img class="image" src="../../../assets/tick.png" alt="tick">
				<app-text :text="text1"></app-text>
			</div>
			<!-- Second sign and text -->
			<div class="text">
				<img class="image" src="../../../assets/cross.png" alt="cross">
				<app-text :text="text2"></app-text>
			</div>
		</div>
	</div>
</div>
</template>

<script>
import Background from '../background/Background.vue';
import Title from '../title/Title.vue';
import Text from '../text/Text.vue';

export default {
	name: "main",
	data() {
		return {
			title: "Free Access to Acme Music",
			text1: "Stream 60 million songs on your device",
			text2: "No internet access"
		}
	},
	components: {
		'app-background': Background,
		'app-title': Title,
		'app-text': Text,
	},
}
</script>

<style>
.main {
	width: 321px;
	height: 299px;
	margin-top: 0px;
}

.main-container {
	width: 321px;
	position: absolute;
	top: 20px;
}

.play {
	width: 321px;
}

.img-play {
	display: block;
	margin: 20px auto;
}

.text-container {
	height: 80px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
	margin-top: 27px;
}

.text {
	display: flex;
	margin: 0;
}

.image {
	display: block;
	width: 12px;
	height: 12px;
	margin-left: 33.5px;
	margin-top: 3px;
}
</style>