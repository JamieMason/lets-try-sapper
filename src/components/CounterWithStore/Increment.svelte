<script>
  import { count } from './store.js';

  const increment = () => {
    count.update(n => n + 1);
  };
</script>

<button type="button" on:click={increment}>+</button>
