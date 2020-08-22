<script>
	let name = 'Maya';
	
	const handleClick = () => {
	  name = 'Gans'
	}
	
	const handleInput = (e) => {
	 name = e.target.value
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>My Single Page Webapp</p>
	<button on:click={handleClick}>update name</button>
	<input type="text" on:input={handleInput}>
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

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>