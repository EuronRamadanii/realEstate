<template>
	<div class="home">
		<div>
			<transition name="fade">
				<div id="pagetop" class="fixed right-0 bottom-0" v-show="scY > 1000" @click="toTop">
					<svg class="test" xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 24 24"
						fill="none" stroke="#4a5568" stroke-width="1" stroke-linecap="square" stroke-linejoin="arcs">
						<path d="M18 15l-6-6-6 6" />
					</svg>
				</div>
			</transition>
		</div>
		<Navigation />
		<Corusel />
		<AboutUs />
		<Services />
		<Projects />
		<Testimonials />
		<!-- <div>
			<TeamCard />
		</div> -->
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
import TeamCard from "../components/TeamCard.vue";
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
		Footer,
		TeamCard
	},
	data() {
		return {
			scTimer: 0,
			scY: 0,
		}
	},
	mounted() {
		window.addEventListener('scroll', this.handleScroll);
	},
	methods: {
		handleScroll: function () {
			if (this.scTimer) return;
			this.scTimer = setTimeout(() => {
				this.scY = window.scrollY;
				clearTimeout(this.scTimer);
				this.scTimer = 0;
			}, 100);
		},
		toTop: function () {
			window.scrollTo({
				top: 0,
				behavior: "smooth"
			});
		},
	},

};
</script>

<style>
#pagetop {
	width: 0
}

.test {
	margin: 1100px 0 0 1850px;
	background-color: #CFB261;
	border-radius: 10px;

}
</style>