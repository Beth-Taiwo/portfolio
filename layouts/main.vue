<template>
	<div class="box-border">
		<div class="relative h-screen w-full overlay">
			<img src="images/photo-1.jpg" class="w-full h-full" alt="" />
		</div>
		<navbar />
		<home />
	</div>
</template>

<script>
import Home from "../components/home.vue";
import navbar from "../components/navbar.vue";
export default {
	components: { navbar, Home },
};
</script>

<style>
.overlay::before {
	content: "";
	position: absolute;
	top: 0;
	left: 0;
	height: 100%;
	width: 100%;
	background: #000;
	opacity: 0.4;
}
</style>
