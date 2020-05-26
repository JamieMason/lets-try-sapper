<script>
  let cities = [{ id: 1, name: 'Hull' }, { id: 2, name: 'Leeds' }];
</script>

<ul>
  {#each cities as { name }}
    <li>{name}</li>
  {/each}
</ul>
