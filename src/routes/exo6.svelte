<style>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
  }

  .grid-container {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
  }

  .col {
    margin-right: 0.5rem;
  }

  .col div {
    background-color: #d78a5f;
    height: 6rem;
    width: 6rem;
    margin-bottom: 0.5rem;
  }

  .semi-square {
    border-radius: 0 50% 0 0;
  }

  .square-circle {
    border-radius: 0 50% 0 50%;
  }

  .semi-circle {
    border-radius: 50% 50% 0 50%;
  }

  .circle {
    border-radius: 50%;
  }

  .circle:last-of-type {
    background-color: black;
  }
</style>

<div class="container">
  <div class="grid-container">
    <div class="col">
      <div class="square" />
      <div class="square" />
      <div class="square" />
      <div class="square" />
      <div class="square" />
    </div>

    <div class="col">
      <div class="semi-square" />
      <div class="semi-square" />
      <div class="semi-square" />
      <div class="semi-square" />
      <div class="semi-square" />
    </div>

    <div class="col">
      <div class="square-circle" />
      <div class="square-circle" />
      <div class="square-circle" />
      <div class="square-circle" />
      <div class="square-circle" />
    </div>

    <div class="col">
      <div class="semi-circle" />
      <div class="semi-circle" />
      <div class="semi-circle" />
      <div class="semi-circle" />
      <div class="semi-circle" />
    </div>

    <div class="col">
      <div class="circle" />
      <div class="circle" />
      <div class="circle" />
      <div class="circle" />
      <div class="circle" />
    </div>
  </div>
</div>
