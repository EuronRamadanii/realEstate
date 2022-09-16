<template>
	<div class="home">
		<Navigation />
		<Corusel />
		<AboutUs />
		<Services />
		<Projects />
		<Testimonials />
		<Contact />
		<Footer />
	</div>
</template>

<script>
import Navigation from "../components/Navbar.vue";
import Corusel from "../components/Corusel.vue";
import AboutUs from "../components/AboutUs.vue";
import Services from "../components/Services.vue";
import Projects from "../components/Projects.vue";
import Testimonials from "../components/Testimonials.vue";
import Contact from "../components/Contact.vue";
import Footer from "../components/Footer.vue";
export default {
	name: "Home",
	components: {
		Navigation,
		Corusel,
		AboutUs,
		Services,
		Projects,
		Testimonials,
		Contact,
		Footer
	},
};
</script>
