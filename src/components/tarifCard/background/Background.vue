<template>
<!-- SVG Background -->
	<svg class="background-svg" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="345.001" height="323.001" viewBox="0 0 345.001 323.001">
		<defs>
			<filter id="Subtraction_2" x="0" y="0" width="345.001" height="323.001" filterUnits="userSpaceOnUse">
				<feOffset dy="5" input="SourceAlpha"/>
				<feGaussianBlur stdDeviation="4" result="blur"/>
				<feFlood flood-opacity="0.502"/>
				<feComposite operator="in" in2="blur"/>
				<feComposite in="SourceGraphic"/>
			</filter>
		</defs>
		<g transform="matrix(1, 0, 0, 1, 0, 0)" filter="url(#Subtraction_2)">
			<path id="Subtraction_2-2" data-name="Subtraction 2" d="M327,299H6V119c3.309,0,6-3.813,6-8.5S9.308,102,6,102V0H327V102a5.263,5.263,0,0,0-4.241,2.493A10.476,10.476,0,0,0,321,110.5c0,4.687,2.692,8.5,6,8.5V299h0Z" transform="translate(6 7)" fill="#fff"/>
		</g>
	</svg>
</template>

<script>
export default {
	name: "background",
}
</script>

<style>
.background-svg {
	position: absolute;
	top: 19px;
	left: -4px;
}
</style>