<script>
	let loggedIn = false
	let name = "Aditya"
	let confirm = false

	function login(){
		loggedIn = true
	}
	function confirmlogout(){
		confirm = false
		loggedIn = false
	}
	function logout(){
		confirm = true
	}
</script>

{#if loggedIn}
	<h1>Hello {name}</h1>
	{#if confirm}
		<h2>are you sure?</h2>
		<button on:click={confirmlogout}> Yes</button>
	{:else}
		<button on:click={logout}>Logout</button>
	{/if}
{:else}
	<h1>Please login to continue</h1>
	<button on:click={login}>Login</button>
{/if} 