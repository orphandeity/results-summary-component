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
    height: 100%;
  }

  @media (min-width: 1024px) {
    main {
      display: grid;
      place-content: center;
      height: 100vh;
    }

    .card {
      width: 768px;
      height: 512px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      border-radius: var(--border-radius);
      box-shadow: 0 30px 60px 0 var(--color-cobalt-blue-shadow);
    }
  }
</style>
