<script>
  let name = '';

  const onSubmit = () => {
    console.log('hello', name);
  };
  const onNameChange = event => {
    name = event.target.value;
  };
</script>

{#if name}
  <p>Hello {name}</p>
{:else}
  <form on:submit|preventDefault={onSubmit}>
    <h1>Introduce yourself:</h1>
    <input type="text" name="name" on:change={onNameChange} />
    <button type="submit">Submit</button>
  </form>
{/if}
