<script>
	export let status;
	export let error;
</script>

<svelte:head>
	<title>Open Sats | Error {status}</title>
</svelte:head>

<div class="container mt-6">
	<h1 class="title">Error {status}</h1>

	<h2 class="subtitle is-uppercase">
		{#if status === 404}Page{/if}
		{error.message}
	</h2>

	<a href="/" class="mt-6 button is-primary">Go back to homepage</a>
</div>
