<script lang="ts">
	// Start of UI language imports

	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-vintage.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';

	// End of UI language imports

	import { goto } from '$app/navigation';

	function goToTypespeedtest(): void {
		goto('/typespeedtest');
	}
</script>

<div class="container mx-auto flex justify-left items-left m-5">
	<h1
		class="text-4xl font-bold text-left"
		on:click={goToTypespeedtest}
		on:keyup={goToTypespeedtest}
	>
		typeOG
	</h1>
</div>

<slot />
