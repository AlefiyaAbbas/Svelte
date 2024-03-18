<script>
	let count = 5
	function incrementCount() {
		count++
	}
</script>

Count is {count}

<button on:click={incrementCount}>Count++</button>