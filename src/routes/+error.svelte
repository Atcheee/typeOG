<script>
	import { goto } from '$app/navigation';
	import { page } from '$app/stores';
	import { onMount } from 'svelte';
	onMount(() => {
		if ($page.status.toString().startsWith('3') || $page.status.toString().startsWith('4')) {
			goto('/typespeedtest');
		}
	});
</script>

<h1>{$page.status}: {$page.error?.message}</h1>
