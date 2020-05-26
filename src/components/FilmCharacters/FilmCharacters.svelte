<script>
  import { onMount } from 'svelte';

  let characters = [];

  onMount(async () => {
    const res = await fetch('https://swapi.co/api/people');
    const json = await res.json();
    characters = json.results;

    return () => {
      console.log('FilmCharacters was unmounted');
    };
  });
</script>

<ul>
  {#each characters as character}
    <li>
      <strong>{character.name}</strong>
    </li>
  {:else}
    <li>...Loading</li>
  {/each}
</ul>
