<script lang="ts">
	import '../app.css';
	import { Toaster } from '$lib/components/ui/sonner/index.js';
	import { ModeWatcher } from 'mode-watcher';
	let { children } = $props();
</script>

<svelte:head>
  <title>My title</title>
  <meta
    name="description"
    content="My description"
  />
</svelte:head>

<ModeWatcher />
<Toaster />
{@render children()}
