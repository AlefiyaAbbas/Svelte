<script>
  let list = ['React', 'Vue']

  function handleClick() {
    list.push('Svelte')
  }
</script>

<p>{list}</p>
<button on:click={handleClick}>Click</button>