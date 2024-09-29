<script>
	import Button from './components/ui/button/button.svelte';
</script>

<nav class="nav-wrapper">
	<div>
		<img src="https://rifrifqyqy.github.io/Tugas-Akhir-RifqyHamdani/images/logo.png" alt="" />
	</div>
	<ul class="menu-nav">
		<li>
			<a href="/">Home</a>
		</li>
		<li>
			<a href="/course">Article</a>
		</li>
		<li>
			<a href="#about">About</a>
		</li>
		<li>
			<a href="#about">Service</a>
		</li>
		<li>
			<a href="#about">Contact</a>
		</li>
		<Button class=" hover:bg-yellow1/80 bg-yellow1 h-12 rounded-lg px-7 text-2xl">Daftar</Button>
	</ul>
</nav>

<style>
	.nav-wrapper {
		@apply bg-green1/90 sticky top-0 z-[9999] flex items-center justify-between px-16 py-5 text-white backdrop-blur-lg;
	}
	.menu-nav {
		@apply flex items-center gap-8 text-lg font-semibold;
	}

	.menu-nav a {
		@apply transition-all duration-300;

		&:hover {
			@apply text-yellow1;
		}
	}
</style>
