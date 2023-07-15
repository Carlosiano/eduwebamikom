<script>
	import '../app.postcss';
	import '../app.css'
	import Analytics from '$lib/analytics.svelte';
</script>

<Analytics />

<slot />

<style>
	:global(html.dark .logo:last-child) {
		fill: #2a5866;
	}
	:global(html .logo:last-child) {
		fill: #113c49;
	}
</style>
