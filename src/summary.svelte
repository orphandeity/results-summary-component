<script lang="ts">
  import data from "./assets/data.json";
</script>

<div class="summary">
  <h2>Summary</h2>
  <ul>
    {#each data as { category, score, icon }}
      <li>
        <div>
          <img src={icon} alt="" />
          {category}
        </div>
        <div class="score">{score} <span>/ 100</span></div>
      </li>
    {/each}
  </ul>
  <button>Continue</button>
</div>

<style>
  .summary {
    padding: 0 30px 30px;
  }
  h2 {
    font-weight: 700;
    color: var(--color-dark-gray-blue);
    margin-block: 24px;
  }
  ul {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }
  li {
    border-radius: var(--border-radius-sm);
    padding: 16px;
    display: flex;
    justify-content: space-between;
  }
  li:first-child {
    background: var(--color-light-red-bg);
    color: var(--color-light-red);
  }
  li:nth-child(2) {
    background: var(--color-orangey-yellow-bg);
    color: var(--color-orangey-yellow);
  }
  li:nth-child(3) {
    background: var(--color-green-teal-bg);
    color: var(--color-green-teal);
  }
  li:nth-child(4) {
    background: var(--color-cobalt-blue-bg);
    color: var(--color-cobalt-blue);
  }

  li div:first-child {
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .score {
    color: var(--color-dark-gray-blue);
    font-weight: 700;
  }
  .score span {
    opacity: 50%;
  }

  button {
    background: var(--color-dark-gray-blue);
    color: var(--color-white);
    border: none;
    border-radius: 9999px;
    padding-block: 16px;
    font-weight: 700;
    width: 100%;
    margin-top: 24px;
  }
  button:hover {
    background: var(--color-cobalt-blue);
    cursor: pointer;
  }
  @media (min-width: 1024px) {
    .summary {
      padding: 0 40px 46px;
    }
    h2 {
      margin: 38px 0 28px;
    }
    button {
      margin-top: 41px;
    }
  }
</style>
