<script>
	const num ='a'
</script>

<main>
	{#if num ===0}
	  <h2>the number is zero</h2>
	{:else if num < 0}
	  <h2>the number is negatives</h2>
	{:else if num > 0}
	  <h2>the number is positve</h2> 
	{:else}
	  <h1>Not a number</h1>
	{/if}
</main>

<style>
	main {
		text-align: center;
		padding: 2em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>