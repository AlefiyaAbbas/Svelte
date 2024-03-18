
<script>
	let loggedIn = false
	let name = "Aditya"

	function login(){
		loggedIn = true
	}

	function logout(){
		loggedIn = false
	}
	
</script>

{#if loggedIn}
	<h1>Hello {name}</h1>
	<button on:click={logout}>Logout</button>
{:else}
	<h1>Please login to continue</h1>
	<button on:click={login}>Login</button>
{/if}