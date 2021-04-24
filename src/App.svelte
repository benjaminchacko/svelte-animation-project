<script>
	let isActive = true;
</script>

<main>
	<h1>Svelte Animation Project</h1>

	<button on:click={() => (isActive = !isActive)}>
		{#if isActive}Hide Box{:else}Show Box{/if}
	</button>
	{#if isActive}
		<div class="box" />
	{/if}
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	.box {
		background: red;
		display: block;
		height: 100px;
		margin: 0 auto;
		width: 100px;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
