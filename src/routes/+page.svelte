<script lang="ts">
	let loaded = false;
</script>

{#if !loaded}
	<div class="loader" />
{/if}

<body class="page1">
	<header>
		<a href="/"> <img src="images/Whatever-Logo.svg" alt="Whatever Social Logo" class="logo"/></a>
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

	<section class="first__section--pg1">
		<div class="banner">
			<div class="hero-elements">
				<h1 class="tagline">
					The best way to get the scoop without creepy
					<span style="color: #db3426">ads</span> &
					<span style="color: #db3426">trackers</span>
				</h1>
				<div class="phone">
					<img
						src="images/Phone.svg"
						alt="Phone showing social media companies being proxied through Whatever Social"
					/>
				</div>
			</div>
			<ul id="scene">
				<img src="images/banner.png" alt="Banner"/>
			</ul>
		</div>
	</section>

	<img src="images/stacked-waves.png" alt="Lavender Waves" class="waves" />

	<section class="second__section--pg1">
		<img id="lock" src="images/whateverlock.gif" alt="Whatever Lock Graphic" />
		<div class="second__section--text">
			<p class="textbox-1">
				"Whatever" represents what we think of your data as a way of income - we don't see you as a
				dollar sign
			</p>
			<div class="cell-2">
				<p class="empty-1" />
			</div>
			<p class="textbox-2">
				With Whatever Social, you can get your social media content with
				<u>no care, no care in the world</u>
			</p>
			<div class="cell-3">
				<p class="empty-2" />
			</div>
		</div>
		<h2 class="textbox-3">
			Your privacy is Whatever's focus. <br /><br />
			Unlike these megacorporations, we don't need to study your viewing habits or searches.
			<br />
			That's <u>WEIRD.</u>
		</h2>
	</section>

	<img src="images/stacked-waves-bottom.svg" alt="Charcoal Waves" class="waves2" />

	<section class="third__section--pg1">
		<div class="container">
			<img
				src="images/Map.svg"
				alt="World map with dots on California US, and Germany"
				class="world-map"
			/>
			<p class="textbox-4">
				Serving thousands of people with servers in 2 continents, we're running on <u>Donations</u>
				and
				<u>Maple Syrup</u>
			</p>
		</div>
	</section>

	<footer>
		<nav class="footerbar">
			<ul class="footer__list">
				<li class="footer__list-logo">
					<img src="images/Whatever-Logo.svg" alt="Whatever Social Small Logo" class="footerlogo" />
				</li>
				<li class="footer__list-item">
					<a href="/privacy" class="nav__link">Privacy Policy</a>
				</li>
				<li class="footer__list-item">|</li>
				<li class="footer__list-item">
					<a href="/transparency" class="nav__link">Transparency Report</a>
				</li>
			</ul>
		</nav>
	</footer>
</body>

<style lang="scss">
	@import '../vars.scss';

	.page1 {
		margin: 0;
		font-family: $font-family_1;
		font-size: 2rem;
		line-height: 1.2;
		color: $color_1;
		background-color: $background-color_1;
	}
	#loading {
		background: var(--clr-black) url(../images/whateverload.gif) no-repeat center center;
		background-size: 10%;
		height: 100vh;
		width: 100%;
		position: fixed;
		z-index: 9999;
		overflow: hidden;
	}
	header {
		background-color: $background-color_2;
		padding: 1em;
		padding-bottom: 0;
		text-align: center;
		margin-top: 0em;
	}
	.logo {
		display: flex;
		margin-left: auto;
		margin-right: auto;
	}
	nav {
		padding: 0;
		margin: 0;
	}
	.navbar {
		min-height: 70px;
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 0 24px;
		padding-top: 0.5em;
		width: 100%;
	}
	.nav__list {
		display: flex;
		justify-content: space-between;
		align-items: center;
		gap: 80px;
		color: $color_1;
		list-style: none;
		font-size: 1.4rem;
		font-weight: var(--fw-normal);
		text-transform: none;
		letter-spacing: 1.5px;
		padding: 0;
	}
	.nav__link {
		text-decoration: none;
		color: $color_2;
		&:hover {
			transition: 0.2s ease;
			color: $color_3;
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
	.hero-elements {
		box-sizing: border-box;
		height: 100vh;
		justify-content: space-between;
		display: flex;
	}
	.tagline {
		float: left;
		max-inline-size: 60%;
		padding-top: 2em;
		color: $color_4;
		letter-spacing: 0px;
		margin-top: 2em;
		margin-left: 2em;
		width: 12em;
		font-size: 3.5rem;
		line-height: 1.2em;
	}
	.phone {
		float: right;
		display: flex;
		justify-content: space-between;
		padding-top: 2em;
		margin-top: 1em;
		width: 100%;
		height: 80%;
		max-width: 700px;
		min-width: 600px;
		max-height: 600px;
		min-height: 400px;
		padding-left: 3em;
		margin-right: 0;
	}
	.banner {
		#scene {
			position: absolute;
			top: 0;
			left: 0;
			right: 0;
			width: 100%;
			height: 250%;
			padding-left: 0.25em;
			overflow: hidden;
			opacity: 10%;
			z-index: -999;
			background: linear-gradient(180deg, rgba(255, 255, 255, 0) 0%, rgba(31, 30, 30, 1) 100%);
		}
	}
	.waves {
		width: 100%;
		height: auto;
		margin-top: -5em;
		vertical-align: middle;
		padding-top: 0;
	}
	.second__section--pg1 {
		height: 100%;
		padding: 0;
		margin: 0;
		color: $color_4;
		background-color: $background-color_4;
		box-sizing: border-box;
		font-family: $font-family_1;
		font-size: 2rem;
		line-height: 1.2;
	}
	#lock {
		height: auto;
		max-width: 50%;
		display: block;
		margin-left: auto;
		margin-right: auto;
		background: url(images/whateverlock.gif) 0 0;
		border-radius: 25px;
	}
	.second__section--text {
		margin-left: 4em;
		margin-right: 4em;
		padding-top: 2em;
		margin-bottom: 2em;
		max-height: 600px;
		display: grid;
		grid-auto-rows: 1fr;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr 1fr 1fr;
		gap: 20px 60px;
		grid-template-areas: 'textbox-1 cell-2' 'cell-3 textbox-2';
	}
	.textbox-1 {
		grid-area: textbox-1;
		text-align: left;
		border-radius: 25px;
		background: #8748aa;
		padding: 20px;
		margin-bottom: 0;
		width: 100%;
		height: 100%;
		box-shadow: -10px 10px white;
	}
	.textbox-2 {
		grid-area: textbox-2;
		text-align: right;
		border-radius: 25px;
		background: #8748aa;
		padding: 20px;
		margin-bottom: 0;
		width: 100%;
		height: 100%;
		box-shadow: 10px 10px white;
	}
	.cell-2 {
		grid-area: cell-2;
	}
	.cell-3 {
		grid-area: cell-3;
	}
	.textbox-3 {
		font-weight: 700;
		text-align: center;
		max-inline-size: unset;
		margin-left: 4em;
		margin-right: 4em;
		margin-top: 0;
		color: $color_4;
		letter-spacing: 0px;
		font-size: 2.5rem;
		line-height: 1.2em;
		margin-bottom: 0;
	}
	.waves2 {
		width: 100%;
		vertical-align: middle;
	}
	.third__section--pg1 {
		display: grid;
		margin-left: 2em;
		margin-right: 2em;
		padding-bottom: 4em;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr;
		gap: 0px 40px;
		grid-template-areas: "world-map textbox-4";
		background-color: $background-color_1;
		font-family: $font-family_1;

		.world-map {
			grid-area: world-map;
			height: auto;
			width: auto;
			max-width: 700px;
		}
		.textbox-4 {
			grid-area: textbox-4;
			line-height: 1.2em;
			text-align: right;
			margin-left: unset;
			margin-right: unset;
			color: $color_4;
			font-size: 2.5rem;
			margin-bottom: 0;
		}
	}
	footer {
		background-color: $background-color_2;
		padding: 1em;
		padding-bottom: 1em;
		text-align: center;
		margin-top: 0em;
		width: 100%;
	}
	.footerbar {
		min-height: 50px;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100%;
	}
	.footer__list {
		display: flex;
		justify-content: space-between;
		align-items: center;
		gap: 80px;
		color: $color_1;
		list-style: none;
		font-size: 1.4rem;
		font-weight: var(--fw-normal);
		text-transform: none;
		letter-spacing: 1.5px;
		padding: 0;
	}
	.footer__list-logo {
		padding-right: 14em;
	}
	.footer__link {
		text-decoration: none;
		color: $color_2;
		&:hover {
			transition: 0.2s ease;
			color: $color_3;
		}
	}
	@media (max-width: 1100px) {
		.burger {
			display: block;
		}
		.bar {
			transition: all 0.2s ease-in-out;
		}
		.burger.active {
			.bar {
				&:nth-child(2) {
					opacity: 0;
				}
				&:nth-child(1) {
					transform: translateY(13px) rotate(45deg);
				}
				&:nth-child(3) {
					transform: translateY(-13px) rotate(-45deg);
				}
			}
		}
		.nav__list {
			opacity: 0;
			position: fixed;
			left: -200vh;
			top: 157.94px;
			gap: 0;
			min-width: 100%;
			height: 50vh;
			flex-direction: column;
			color: $color_4;
			background-color: $background-color_1;
			padding-top: 1em;
			padding-bottom: 1em;
			text-align: center;
			align-items: center;
		}
		.nav__link {
			margin: 0;
		}
		.nav__list.active {
			left: 0;
			margin: 0;
			opacity: 100%;
		}
	}
	@media (max-width: 1350px) {
		.hero-elements {
			font-size: 2rem;
			color: $color_4;
			justify-content: unset;
			display: inline-block;
			padding: 2em 0.8em;
			padding-top: 5em;
			padding-bottom: 0;
			box-sizing: border-box;
			height: 100%;
			text-align: center;
			align-items: center;
		}
		.banner {
			#scene {
				opacity: 0;
			}
		}
		.waves {
			margin-top: 0;
		}
		.phone {
			float: unset;
			display: block;
			text-align: center;
			justify-content: space-between;
			padding-top: 3em;
			width: unset;
			height: unset;
			max-width: unset;
			min-width: unset;
			max-height: unset;
			padding-left: unset;
		}
		.tagline {
			display: inline;
			max-inline-size: unset;
			padding-top: unset;
			color: $color_4;
			letter-spacing: unset;
			margin-top: unset;
			margin-left: unset;
			width: unset;
			font-size: 2.5rem;
			float: unset;
			line-height: 1.2em;
		}
		.second__section--text {
			display: grid;
			justify-content: center;
			align-items: center;
			margin-left: 2em;
			margin-right: 2em;
			grid-auto-rows: 1fr;
			grid-template-columns: 1fr;
			grid-template-rows: 1fr;
			gap: 20px 40x;
			grid-template-areas: 'textbox-1' 'textbox-2';
		}
		.textbox-1 {
			grid-area: textbox-1;
			text-align: center;
			box-shadow: 0px 10px white;
		}
		.textbox-2 {
			grid-area: textbox-2;
			text-align: center;
			box-shadow: 0px 10px white;
		}
		.cell-2 {
			grid-area: cell-2;
			display: none;
		}
		.cell-3 {
			grid-area: cell-3;
			display: none;
		}
		.textbox-3 {
			text-align: center;
			max-inline-size: unset;
			color: $color_4;
			letter-spacing: unset;
			font-size: 2rem;
			margin-left: 1.5em;
			margin-right: 1.5em;
			margin-top: 10em;
			margin-bottom: unset;
			float: unset;
			width: unset;
			line-height: 1em;
		}
		.third__section--pg1 {
			display: grid;
			margin-left: 2em;
			margin-right: 2em;
			padding-bottom: 4em;
			align-items: center;
			justify-items: center;
			grid-template-columns: 1fr;
			gap: 0px 40px;
			grid-template-areas: 'world-map' 'textbox-4';
		}
		.world-map {
			display: block;
			text-align: center;
			justify-content: center;
			width: 100%;
			height: auto;
		}
		.textbox-4 {
			text-align: center;
			margin-left: 1em;
			margin-right: 1em;
			color: $color_4;
			font-size: 1.5rem;
			margin-bottom: 0;
		}
		.footer__list-logo {
			display: none;
		}
		.footer__list {
			gap: 40px;
			font-size: 1rem;
			letter-spacing: 1.5px;
		}
	}
	@media (max-width: 400px) {
		.phone {
			max-width: 300px;
		}
	}
	@media (min-width: 1900px) {
		.phone {
			margin-right: 4em;
		}
		.tagline {
			margin-left: 4em;
		}
	}
	@media (max-width: 600px) {
		#lock {
			max-width: 70%;
		}
	}
</style>
