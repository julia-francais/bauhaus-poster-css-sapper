<style>
  .container {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
  }

  .col {
    background-color: #e1b09e;
    height: 30%;
    width: 8%;
    display: inline-block;
    border-radius: 0 0 8rem;
    margin-right: 0.3rem;
    position: relative;
  }
  .col:nth-of-type(1) {
    border-radius: 0 0 0 8rem;
  }

  .col:nth-of-type(2) {
    width: 10%;
    height: 45%;
    background-color: #d8987d;
  }

  .circle {
    border-radius: 50%;
    position: absolute;
    bottom: 3rem;
    transform: translateX(-50%);
  }

  .col:nth-of-type(2) .circle {
    width: 3rem;
    height: 3rem;
    background-color: #e1afa0;
  }

  .col:nth-of-type(3) {
    width: 15%;
    height: 60%;
    background-color: #e1afa0;
  }

  .col:nth-of-type(3) .circle {
    width: 6rem;
    height: 6rem;
    background-color: #fab14f;
  }

  .col:nth-of-type(4) {
    width: 25%;
    height: 75%;
    background-color: #fab14f;
  }

  .col:nth-of-type(4) .circle {
    width: 5rem;
    height: 5rem;
    bottom: 2rem;
    background-color: #e1afa0;
  }
</style>

<div class="container">
  <div class="col" />
  <div class="col">
    <div class="circle" />
  </div>
  <div class="col">
    <div class="circle" />
  </div>
  <div class="col">
    <div class="circle" />
  </div>
</div>
