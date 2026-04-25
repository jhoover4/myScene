<script>
	import '../app.css';
	import { resolve } from '$app/paths';
	import { page } from '$app/state';
	import { locales, localizeHref } from '$lib/paraglide/runtime';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="container">
  <nav class="site-nav">
    <h1 class="logo">myScene</h1>
		<div class="nav-links">
			<a href="/">Home</a>
			<a href="/artists">Artists</a>
			<a href="/fans">Fans</a>
			<a href="/venues">Venues</a>
			<a href="/investors">Community Investors</a>
		</div>
	</nav>

	{@render children()}
</div>