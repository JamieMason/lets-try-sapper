<script>
  import { count } from './store.js';
  import Increment from './Increment.svelte';
  import Decrement from './Decrement.svelte';
  import Replace from './Replace.svelte';
</script>

<h1>The count is {$count}</h1>

<Increment />
<Decrement />
<Replace />
