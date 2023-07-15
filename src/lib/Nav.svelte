<script lang="ts">
	import IoLogoGithub from 'svelte-icons/io/IoLogoGithub.svelte';
	import FaMastodon from 'svelte-icons/fa/FaMastodon.svelte';
</script>

<header>
	<a href="/"> <img src="images/Whatever-Logo.svg" alt="Whatever Social Logo" class="logo" /></a>
	<nav class="navbar">
		<ul class="nav__list">
			<li>
				<a href="https://launch.whatever.social" class="nav__link">Frontends & Tools</a>
			</li>
			<!-- <li class="nav__list-item">
				<a href="/guides" class="nav__link">Guides</a>
			</li> -->
			<li class="nav__list-item">
				<a href="/contact" class="nav__link">Contact</a>
			</li>
			<li class="nav__list-item">
				<a href="/donate" class="nav__link">Donate</a>
			</li>
			<li class="nav__list-item">
				<a href="https://status.whatever.social/status/live" class="nav__link">Status</a>
			</li>
			<li class="nav__list-item">
				<a
					href="https://github.com/WhateverLabs/WhateverSite"
					target="_blank"
					rel="noopener noreferrer"
					class="nav__link"
				>
					<div style="height: 1.5rem; width: 1.5rem;">
						<IoLogoGithub />
					</div>
				</a>
			</li>
			<li class="nav__list-item">
				<a
					href="https://orchard.social/@whatever"
					target="_blank"
					rel="me"
					class="nav__link"
				>
					<div style="height: 1.5rem; width: 1.5rem;">
						<FaMastodon />
					</div>
				</a>
			</li>
		</ul>
	</nav>
</header>

<style lang="scss">
	@import '../vars.scss';

	header {
		background-color: $background-color_2;
		padding: 1em;
		padding-bottom: 0;
		text-align: center;
		margin-top: 0em;
	}

	.navbar {
		min-height: 70px;
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 0 24px;
		padding-top: 0.5em;
		width: 100%;
		.nav__list {
			display: flex;
			justify-content: space-between;
			align-items: center;
			gap: 2rem;
			color: $color_1;
			list-style: none;
			font-size: 1.4rem;
			font-weight: var(--fw-normal);
			text-transform: none;
			padding: 0;
			flex-wrap: wrap;

			@media only screen and (max-width: $mobile-width) {
				font-size: 1.2rem;
			}

			.nav__link {
				text-decoration: none;
				color: $color_2;
				&:hover {
					transition: 0.2s ease;
					color: $color_3;
				}

				.nav__list-item {
					margin: 0;
				}
			}
		}
	}
</style>
