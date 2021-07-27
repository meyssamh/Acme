<template>
<!-- Actionbutton -->
	<button class="action">
		<!-- Actionbutton's text -->
		<h1 class="action-title">{{ actionTitle }}</h1>
	</button>
</template>

<script>
export default {
	name: "action",
	props: {
		actionTitle: String,
	},
}
</script>

<style>
.action {
	width: 321px;
	height: 106px;
	border-radius: 0 0 14px 14px;
	box-shadow: 0 5px 8px 0 rgba(0, 0, 0, 0.5);
	background-image: linear-gradient(to right, #b7f1c1, #b1e6de);
	border: none;
	cursor: pointer;
	position: absolute;
	margin-top: 18px;
}

.action-title {
	font-weight: 700;
	color: #08144a;
}
</style>