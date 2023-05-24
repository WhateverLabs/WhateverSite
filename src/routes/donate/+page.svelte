<script lang="ts">
	const copyMonero = () => {
		try {
			navigator.permissions
				.query({
					// @ts-ignore
					name: 'clipboard-write'
				})
				.then((r) => {
					if (r.state == 'granted' || r.state == 'prompt')
						navigator.clipboard
							.writeText(
								'87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7'
							)
							.then(function (m) {
								alert('The Monero address was beamed to your device. Paste away!');
							});
					else
						try {
							navigator.clipboard
								.writeText(
									'87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7'
								)
								.then(function (m) {
									alert(
										"Whoops, we're not sure if this copied in your browser. Here's the address just in case: 87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7"
									);
								});
						} catch {
							alert(
								"For some reason we couldn't copy the Monero address to your clipboard. Here's the ID: 87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7"
							);
						}
				});
		} catch {
			navigator.clipboard
				.writeText(
					'87tu5QTMSKmi8RmyyRCP1daBouRKegmL54k9d4cqqWscHWTqSaKRXQu9X2g81JgJyfQFbyL1dTRmR6TsZ8oZZqLj1Ljfyd7'
				)
				.then(function (m) {
					alert('The Monero address was beamed to your device. Paste away!');
				});
		}
	};
</script>

<div class="content">
	<div class="child">
		<p>
			As a student, mounting server costs may become a problem in the future. If you'd like to
			support this project's growth, please consider donating via <a
				href="https://liberapay.com/whateversocial"
				target="_blank"
				rel="noopener noreferrer">Liberapay</a
			>
			or <a href="#" on:click={copyMonero}>Monero</a>.
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

		box-sizing: border-box;
		padding: 5rem;

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
</style>
