<template>
	<div id="nav">
		<!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
		<Home />
	</div>
	<router-view />
</template>
<script>
import Home from "./views/Home.vue";
export default {
	components: { Home },
	// mounted() {
	// 	AOS.init()
	// },
};
</script>

