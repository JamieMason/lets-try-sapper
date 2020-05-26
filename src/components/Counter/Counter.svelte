<script>
  let count = 0;
  $: squared = count ** 2;
  $: squaredMinusOne = squared - 1;

  const onClick = () => {
    count++;
  };
</script>

<style>
  .number {
    font-weight: bold;
  }
</style>

<p>
  <button on:click={onClick}>Counter: {count}</button>
  Squared is
  <span class="number">{squared}</span>
  | Squared minus 1 is
  <span class="number">{squaredMinusOne}</span>
</p>
