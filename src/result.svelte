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
    font-size: 24px;
    font-weight: 700;
    color: var(--color-white);
  }

  p {
    font-size: 16px;
    color: var(--color-light-lavendar);
    text-align: center;
    max-width: 260px;
  }

  .circle {
    border-radius: 9999px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: var(--gradient-2);
    width: 140px;
    aspect-ratio: 1/1;
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
  @media (min-width: 1440px) {
    h1 {
      font-size: 24px;
    }
    h2 {
      font-size: 32px;
    }
    p {
      font-size: var(--font-size);
    }
    .result {
      border-radius: var(--border-radius);
      gap: 0;
    }
    .result > :nth-child(2) {
      margin-top: 35px;
    }
    .result > :nth-child(3) {
      margin-top: 27px;
    }
    .result > :last-child {
      margin-top: 14px;
    }
    .circle {
      width: 200px;
      gap: 4px;
    }
    .circle :first-child {
      font-size: 72px;
    }
    .circle :last-child {
      font-size: var(--font-size);
    }
  }
</style>
