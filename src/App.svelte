<script>
  import Result from "./result.svelte";
  import Summary from "./summary.svelte";
</script>

<main>
  <div class="card">
    <Result />
    <Summary />
  </div>
</main>

<style>
  .card {
    background: var(--color-white);
    height: 100vh;
  }
</style>
