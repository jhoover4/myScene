<script>
	let { header, subheading, linkText, link } = $props();
</script>
<section class="page-hero">
	<h2>{header}</h2>
	<p>{subheading}</p>
{#if linkText }
	<a href="{link}" class="btn">{ linkText }</a>
{/if}
</section>