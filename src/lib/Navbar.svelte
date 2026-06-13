<script lang="ts">
	let menuOpen = $state(false);
</script>

<!-- Top bar: visible on small screens, hidden at 1020px+ -->
<header class="navbar">
	<div class="navbar-title">
		<a href="/" class="navbar-title-link">
			<span class="site-name">Ricco Cruz</span>
		</a>
	</div>
	<div class="navbar-container">
		<section class="navbar-section">
			<button
				class="navbar-button nav-menu-button"
				onclick={() => (menuOpen = !menuOpen)}
				aria-label="Toggle menu"
				aria-expanded={menuOpen}
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
				>
					<path d="M3 12h18" /><path d="M3 18h18" /><path
						d="M3 6h18"
					/>
				</svg>
			</button>
			<nav class="navbar-menu nav-items" class:active={menuOpen}>
				<a href="#projects" onclick={() => (menuOpen = false)}
					>Projects</a
				>
				<a href="#about" onclick={() => (menuOpen = false)}>About</a>
			</nav>
			<nav class="navbar-menu social">
				<a
					href="https://github.com/riccocruz"
					class="navbar-button"
					target="_blank"
					rel="noopener noreferrer"
					><i class="fa-solid fa-code"></i> GitHub</a
				>
			</nav>
			<nav class="navbar-menu social">
				<a
					href="https://github.com/riccocruz"
					class="navbar-button"
					target="_blank"
					rel="noopener noreferrer"
					><i class="fa-brands fa-linkedin-in"></i> LinkedIn</a
				>
			</nav>
		</section>
	</div>
</header>

<!-- Left sidebar: hidden on small screens, visible at 1020px+ -->
<aside class="sidebar">
	<section class="sidebar-section">
		<a href="/" class="site-name">Ricco Cruz</a>
		<p>software builder</p>
	</section>
	<section class="sidebar-section">
		<nav class="sidebar-nav-links">
			<a href="#projects">Projects</a>
			<a href="#about">About</a>
		</nav>
	</section>
	<section class="sidebar-section">
		<nav class="sidebar-nav-links">
			<a
				href="https://github.com/riccocruz"
				target="_blank"
				rel="noopener noreferrer"
				><i class="fa-solid fa-code"></i> GitHub</a
			>
			<a
				href="https://www.linkedin.com/in/riccoveigh/"
				target="_blank"
				rel="noopener noreferrer"
				><i class="fa-brands fa-linkedin-in"></i>LinkedIn</a
			>
		</nav>
	</section>
</aside>
