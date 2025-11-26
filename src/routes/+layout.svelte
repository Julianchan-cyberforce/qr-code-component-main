<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
  import { base } from '$app/paths';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="navbar bg-base-100 shadow-sm">
  <a href="{base}/" class="btn btn-ghost text-xl">Home</a>
  <a href="{base}/qr-code" class="btn btn-ghost text-xl">QRcode</a>
</div>
{@render children()}
