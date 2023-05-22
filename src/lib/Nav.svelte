<header>
	<a href="/"> <img src="images/Whatever-Logo.svg" alt="Whatever Social Logo" class="logo" /></a>
	<nav class="navbar">
		<ul class="nav__list">
			<li class="nav__list-item">
				<a href="/socials" class="nav__link">Social Frontends</a>
			</li>
			<li class="nav__list-item">
				<a href="/knowledge" class="nav__link">Knowledge Frontends</a>
			</li>
			<li class="nav__list-item">
				<a href="/tools" class="nav__link">Tools</a>
			</li>
			<li class="nav__list-item">
				<a href="/guides" class="nav__link">Guides</a>
			</li>
			<li class="nav__list-item">
				<a href="/contact" class="nav__link">Contact</a>
			</li>
			<li class="nav__list-item">
				<a href="/donate" class="nav__link">Donate</a>
			</li>
		</ul>
		<div class="burger">
			<span class="bar" />
			<span class="bar" />
			<span class="bar" />
		</div>
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
				/* flex-wrap: wrap; */
			}

			.nav__link {
				text-decoration: none;
				color: $color_2;
				&:hover {
					transition: 0.2s ease;
					color: $color_3;
				}
			}
		}
	}

	.burger {
		display: none;
		cursor: pointer;
		padding-bottom: 0.5em;
	}
	.bar {
		display: block;
		width: 40px;
		height: 6px;
		margin: 7px auto;
		background-color: $background-color_3;
	}
</style>
