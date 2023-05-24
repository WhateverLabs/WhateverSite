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

<style lang="scss">
	@import '../vars.scss';

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

			@media screen and (max-width: $mobile-width) {
				flex-direction: column;
			}
		}
		.footer__link {
			text-decoration: none;
			color: $color_2;
			&:hover {
				transition: 0.2s ease;
				color: $color_3;
			}
		}
	}
</style>
