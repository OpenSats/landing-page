<script>
	import { onMount } from 'svelte';
	import { fade } from 'svelte/transition';

	import Navbar from '../components/layout/Navbar.svelte';

	let visible = false;
	let mobileMenuOpen = false;

	const handleMobileMenuOpen = () => {
		mobileMenuOpen = true;
	};

	const handleMobileMenuClose = () => {
		mobileMenuOpen = false;
	};

	onMount(() => {
		visible = true;
	});
</script>

{#if visible}
	<div in:fade={{ duration: 721 }} class:is-height-limited={mobileMenuOpen}>
		<Navbar on:menuOpen={handleMobileMenuOpen} on:menuClose={handleMobileMenuClose} />

		<main>
			<slot />
		</main>
	</div>
{/if}

<style lang="sass" global>
	@import '../main.sass'

	main
		overflow-x: hidden !important
		max-width: 100vw !important

	.is-height-limited
		overflow: hidden !important
		max-height: 92vh !important
</style>
