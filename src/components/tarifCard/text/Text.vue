<template>
	<!-- Tarif texts -->
	<p class="main-text">{{ text }}</p>
</template>

<script>
export default {
	name: "main-text",
	props: {
		text: String
	},
}
</script>

<style>
.main-text {
	width: 206px;
	font-weight: 500;
	text-align: left;
	color: #262626;
	margin: 0 0 0 11.5px;
}
</style>