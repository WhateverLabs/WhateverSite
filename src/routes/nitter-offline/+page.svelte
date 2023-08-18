<div class="content">
	<div class="child">
		<h3>Our Nitter instance was shut down on August 17, 2023</h3>
        <p>
			Due to increasingly severe shortcomings of Twitter's moderation team, 
            we shut down our Nitter instance. A 3-week warning was posted on our
            <a href="https://orchard.social/@whatever/110788570817924842" class="link">Mastodon</a>.
        </p>
        <p>    
            A list of other Nitter instances are available 
            <a href="https://github.com/zedeus/nitter/wiki/Instances" class="link">here</a>. 
        </p>
        <p>    
            Alternatively, you can use our <a href="https://orchard.social" class="link">Mastodon instance</a>, 
            where you can search for <code>@twitter_username@bird.makeup</code> and add their new posts to your feed.  
            For example, if you wanted to follow Playstation, you can follow <code>@playstation@bird.makeup</code>. 
            But, you're encouraged to discover new Fediverse accounts, as those are the ones trying out a 
            new frontier of social media.
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
