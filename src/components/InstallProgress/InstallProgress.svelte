<script>
  import { cubicOut } from 'svelte/easing';
  import { tweened } from 'svelte/motion';
  const progress = tweened(0, {
    duration: 5000,
    easing: cubicOut
  });
</script>

<style>
  progress {
    display: block;
    width: 100%;
  }
</style>

{#if $progress === 1}
  <h1>Installation Complete</h1>
{:else}
  <h1>Installing Windows 95</h1>
  <progress value={$progress} />
  <sub>2 weeks remaining...</sub>

  <button type="text" on:click={() => progress.set(0)}>0%</button>
  <button type="text" on:click={() => progress.set(0.75)}>75%</button>
  <button type="text" on:click={() => progress.set(1)}>100%</button>
{/if}
