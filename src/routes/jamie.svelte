<script>
  import Cities from '../components/Cities/Cities.svelte';
  import Counter from '../components/Counter/Counter.svelte';
  import CounterWithStore from '../components/CounterWithStore/CounterWithStore.svelte';
  import FilmCharacters from '../components/FilmCharacters/FilmCharacters.svelte';
  import InstallProgress from '../components/InstallProgress/InstallProgress.svelte';
  import IntroForm from '../components/IntroForm/IntroForm.svelte';
  import UserInfo from '../components/UserInfo/UserInfo.svelte';
</script>

<svelte:head>
  <title>Svelte Spike</title>
</svelte:head>

<UserInfo />
<Counter />
<hr />
<CounterWithStore />
<hr />
<FilmCharacters />
<Cities />
<IntroForm />
<InstallProgress />
