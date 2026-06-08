<script>
	import '../app.css';
	import { resolve } from '$app/paths';
	import { page } from '$app/state';
	import { locales, localizeHref } from '$lib/paraglide/runtime';
	import favicon from '$lib/assets/favicon.png';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="container">
  <nav class="site-nav">
    <h1 class="logo">myScene</h1>
		<div class="nav-links">
			<a href="{resolve('/')}">Home</a>
			<a href="{resolve('/artists')}">Artists</a>
			<a href="{resolve('/fans')}">Fans</a>
			<a href="{resolve('/venues')}">Venues</a>
			<a href="{resolve('/investors')}">Community Investors</a>
		</div>
	</nav>

	{@render children()}
</div>
<footer class="site-footer">
  <div class="container">
    <div class="site-footer-inner">
	<a target="_blank" href="https://icons8.com/icon/25081/drums" class="link">Drum Set</a> icon by <a target="_blank" href="https://icons8.com" class="link">Icons8</a>
    </div>
  </div>
</footer>