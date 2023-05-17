<script>
	let count = 0;

	function handleIncrement() {
		count++;
	}

	let items = ['Milk', 'Sugar', 'Horlicks', 'Eno', 'Mango', 'Cashew', 'Tea', 'Besan'];
</script>

<h1>{count}</h1>
<button on:click={handleIncrement}>Increment</button>

{#each items as item, index (item)}
	<h2>{index + 1}. {item}</h2>
{/each}
