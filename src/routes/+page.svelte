<script lang="ts">
	let loaded = false;
</script>

{#if !loaded}
	<div class="loader" />
{/if}

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
					src="images/whatever_phones.png"
					alt="Phones showing social media companies being proxied through Whatever Social, Whatever Launchpad, and AO"
				/>
			</div>
		</div>
	</div>
</section>

<img src="images/stacked-waves.png" alt="Lavender Waves" class="waves" />

<section class="second__section--pg1">
	<img id="lock" src="/images/whateverlock.gif" alt="Whatever Lock Graphic" />
	<div class="second__section--text">
		<div class="container left">
			<p class="textbox">
				Whatever Social is a collection of FOSS alternative frontends and self-hosted services to try 
				and close the gap between viewing mainstream social media and privacy
			</p>
		</div>
		<div class="container right">
			<p class="textbox">
				With Whatever Social, you can get your social media content with
				<u>no care, no care in the world</u>
			</p>
		</div>
		<div class="container left 2">
			<p class="textbox">
				"Whatever" represents what we think of your data as a way of income - we don't see you as a
				dollar sign
			</p>
		</div>
	</div>
	<h2 class="focus">
		Because unlike these mega-corporations, we don't need to study your viewing habits or searches.
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

<style lang="scss">
	@import '../vars.scss';

	#loading {
		background: var(--clr-black) url(../images/whateverload.gif) no-repeat center center;
		background-size: 10%;
		height: 100vh;
		width: 100%;
		position: fixed;
		z-index: 9999;
		overflow: hidden;
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
	.hero-elements {
		height: 100vh;
		justify-content: space-between;
		display: flex;
		width: 100%;
		padding: 3rem;
		box-sizing: border-box;
		align-items: center;

		background-image: linear-gradient(to bottom, #00000095, #201e1e 90%), url('/images/banner.png');
		background-size: cover;

		@media only screen and (max-width: $mobile-width) {
			display: inline-block;
			padding: 1rem;
		}
	}
	.tagline {
		color: $color_4;
		letter-spacing: 0px;
		font-size: 3.5rem;
		line-height: 1.2em;
	}

	.first__section--pg1 {
		width: 100%;
	}
	.phone {
		width: 100%;

		display: flex;
		align-items: center;
		img {
			width: 100%;
		}
	}
	.waves {
		width: 100%;
		height: auto;
		vertical-align: middle;
		padding-top: 0;
		z-index: 3;
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

		@media only screen and (max-width: $mobile-width) {
			display: block;
		}

		padding: 3rem;
		box-sizing: border-box;

		.second__section--text {
			.container {
				width: 100%;
				&.right {
					display: flex;
					justify-content: flex-end;
				}
				.textbox {
					text-align: left;
					border-radius: 25px;
					background: #8748aa;
					padding: 20px;
					margin-bottom: 0;
					width: 35rem;
					height: 100%;
					box-shadow: -10px 10px white;
					box-sizing: border-box;
					box-sizing: border-box;

					@media only screen and (max-width: $mobile-width) {
						width: 100%;
					}
				}
			}
		}
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
	.cell-2 {
		grid-area: cell-2;
	}
	.cell-3 {
		grid-area: cell-3;
	}

	.waves2 {
		width: 100%;
		vertical-align: middle;
	}
	.third__section--pg1 {
		.container {
			display: flex;
			padding: 2rem;
			box-sizing: border-box;
			flex-wrap: wrap;
			@media only screen and (max-width: $mobile-width) {
				/* display: block; */
			}

			.world-map {
				height: auto;
				width: auto;
				max-width: 700px;

				@media only screen and (max-width: $mobile-width) {
					width: 100%;
				}
			}
			.textbox-4 {
				color: $color_4;
				text-align: right;
				font-size: 2.5rem;
				margin-bottom: 0;
			}
		}

		background-color: $background-color_1;
		font-family: $font-family_1;
	}
</style>
