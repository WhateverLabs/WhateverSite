<div class="content">
	<div class="child">
		<p>
			As students, mounting server costs may become a problem in the future. If you'd like to
			support this project's growth, please consider donating via <a
				href="https://liberapay.com/whateversocial"
				class="link"
				target="_blank"
				rel="noopener noreferrer">Liberapay</a
			>
			or Monero (<code>87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7</code>).
		</p>

		<h3>About</h3>
		<p>
			Whatever Social was started in July of 2022 to help give people an option to use some of
			their social media privately through open-source alternative frontends. Since then, we've
			slowly expanded to services like Vaultwarden and even our own hosted social media like Mastodon.
			Not only did the amount of services increase, but our network of servers has also completely
			shifted around and become more capable than ever. We've also made our own mark by designing
			and developing our own StackOverflow frontend, and our own website firewall.
			As we continue to build up our own corner of the privacy space, and as more people discover us, 
			costs of running Whatever and its branches increase. We don't (and will never) run ads, and rely 
			solely on donations to keep the service up. Soon, we'll post a public report of monthly costs. 
			Thanks for using Whatever.
		</p>
	</div>
</div>

<style lang="scss">
	@import '../../vars.scss';

	.content {
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;

		font-size: 24px;
		box-sizing: border-box;
		padding: 5rem;
		padding-left: 6em;
		padding-right: 6em;

		@media only screen and (max-width: $mobile-width) {
			padding: 1rem;
		}

		code {
			word-break: break-all;
			background-color: #353535;
			box-sizing: border-box;
			width: 100%;
		}
	}
	.link {
		color: $color_3;
	}
</style>
