<script lang="ts">
	import Footer from '$lib/Footer.svelte';
	import Nav from '../lib/Nav.svelte';
	import '../main.scss';
</script>

<svelte:head>
	<title>Whatever Social</title>
	<meta
		name="description"
		content="Premium self-hosted instances of popular social media frontends. The best way to get the scoop without creepy ads & trackers."
	/>
	<meta name="og:image" content="/images/favicon.png" />
	<meta name="theme-color" content="#ffffff" />
</svelte:head>

<Nav />
<slot />
<Footer />
