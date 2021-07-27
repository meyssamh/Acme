<template>
	<!-- Tarif title -->
	<h1 class="title">{{ mainTitle }}<small class="registered">&reg;</small></h1>
</template>

<script>
export default {
	name: "main-title",
	props: {
		mainTitle: String,
	}
}
</script>

<style>
.title {
	width: 220px;
	font-weight: 700;
	text-align: center;
	color: #08144a;
	margin: 20px auto;
}

.registered {
	font-size: 12px;
	vertical-align: super;
}
</style>