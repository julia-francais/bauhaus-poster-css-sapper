<style>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
  }
  .circle {
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .circle:first-of-type {
    height: 26rem;
    width: 26rem;
    background-color: #27366d;
    z-index: 1;
  }

  .circle .circle {
    height: 20rem;
    width: 20rem;
    background-color: #1c2952;
    z-index: 2;
  }

  .circle .circle .circle {
    height: 12rem;
    width: 12rem;
    background-color: #0f1330;
    z-index: 3;
  }

  .circle .circle .circle .circle {
    height: 6rem;
    width: 6rem;
    background-color: black;
    z-index: 6;
  }
</style>

<div class="container">
  <div class="circle">
    <div class="circle">
      <div class="circle">
        <div class="circle" />
      </div>
    </div>
  </div>
</div>
