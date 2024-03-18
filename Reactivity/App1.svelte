<script>
	let prizes = [100, 200, 300]

	function addPrice(){
		prizes = [...prizes, 500]
		console.log(prizes)
	}

	$: grandtotal = prizes.reduce((a,b)=>a+b, 0)
</script>

<h1>The Grand Total is: {grandtotal}</h1>

<button on:click={addPrice}>Add 500</button>
