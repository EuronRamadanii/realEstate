<template>
	<div class="home">
		<Navigation />
		<!-- <Corusel /> -->
		<AboutUs />
	</div>
</template>

<script>
import Navigation from "../components/Navbar.vue";
import Corusel from "../components/Corusel.vue";
import AboutUs from "../components/AboutUs.vue";
export default {
	name: "Home",
	components: {
		Navigation,
		Corusel,
		AboutUs,
	},
};
</script>
