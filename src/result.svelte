<div class="result">
  <h1>Your Result</h1>
  <div class="circle"><span>76</span><span>of 100</span></div>

  <h2>Great</h2>
  <p>Your performance exceeds 65% of the people conducting the test here!</p>
</div>

<style>
  h1 {
    color: var(--color-light-lavendar);
  }
  h2 {
    font-weight: 700;
  }
  p {
    font-size: 16px;
    color: var(--color-light-lavendar);
    max-width: 260px;
    text-align: center;
  }
  .circle {
    border-radius: 9999px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: var(--gradient-2);
    width: 140px;
    height: 140px;
  }
  .circle :first-child {
    font-size: 56px;
    font-weight: 800;
    line-height: 72px;
    color: var(--color-white);
  }
  .circle :last-child {
    font-size: 16px;
    color: var(--color-light-lavendar);
  }

  .result {
    background: var(--gradient-1);
    border-bottom-left-radius: var(--border-radius);
    border-bottom-right-radius: var(--border-radius);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 24px;
    padding-bottom: 40px;
    padding-top: 24px;
  }
  .result h2 {
    font-size: 24px;
    color: var(--color-white);
  }
</style>
