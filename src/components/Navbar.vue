<template>
	<nav id="navbar" class="navbar navbar-expand-sm">
		<div class="container">
			<a class="navbar-brand" href="#">
				<img src="../assets/images/logo.png" alt="logo detail" />
			</a>
			<button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbar-main">
				<span class="navbar-toggler-icon"><i class="fas fa-bars"></i></span>
			</button>
			<div class="collapse navbar-collapse" id="navbar-main">
				<ul class="navbar-nav ml-auto mb-2 mb-lg-0">
					<li class="nav-item">
						<a class="nav-link active" href="#about">About</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#services">Services</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#projects">Projects</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#testimonials">Testimonials</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#contact">Contact</a>
					</li>
				</ul>
			</div>
		</div>
	</nav>
</template>

<script>
// import style from "../assets/style.css";
export default {
	name: "Navbar",
};
</script>

<!-- <style scoped>
* {
	padding: 0;
	margin: 0;
	font-family: "Ubuntu", sans-serif;
	font-weight: 300;
}

.navbar {
	position: absolute !important;
	width: 100%;
	z-index: 2;
}

.navbar-brand img {
	max-width: 240px;
}

.navbar-nav {
	margin-left: auto;
}

.nav-link {
	font-weight: 500;
	margin: 0 10px;
	color: var(--color-light2) !important;
}

.nav-link:hover {
	color: var(--color-light) !important;
}

.navbar-toggler {
	border-color: #fff !important;
}

.navbar-toggler-icon {
	padding: 5px 0;
}

.navbar-toggler-icon i {
	color: #fff;
}

.fixed {
	position: fixed !important;
	top: 0;
	width: 100%;
	background-color: var(--color-dark);
	z-index: 4;
}
</style> -->
