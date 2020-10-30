<style>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .half-circle {
    background-color: #fdbb63;
    position: relative;
  }

  .left {
    margin-top: 15rem;
    margin-right: 2.5rem;
    height: 25rem;
    width: 12.5rem;
    border-radius: 12.5rem 0 0 12.5rem;
  }

  .right {
    margin-bottom: 6rem;
    height: 17rem;
    width: 8.5rem;
    border-radius: 0 8.5rem 8.5rem 0;
    z-index: 4;
  }

  .half-circle .circle::before {
    content: "";
    position: absolute;
    border-radius: 50%;
    background-color: #e2b1a1;
    z-index: 5;
  }

  .left.half-circle .circle::before {
    height: 8rem;
    width: 8rem;
    position: absolute;
    transform: translate(3rem, -55%);
  }

  .left.half-circle .circle {
    top: 0;
    right: 0;
    transform: translate(7rem, 13rem);
    content: "";
    position: absolute;
    border-radius: 0 0 7rem 7rem;
    background-color: #e18954;
    z-index: 3;
    bottom: 0;
    height: 7rem;
    width: 14rem;
  }

  .right.half-circle .circle::before {
    transform: translate(2rem, 2.5rem);
    height: 5rem;
    width: 5rem;
  }

  .right.half-circle .circle {
    top: 0;
    right: 0;
    transform: translate(-3rem, 3.5rem);
    content: "";
    position: absolute;
    border-radius: 4.5rem 4.5rem 0 0;
    background-color: #e18954;
    z-index: 3;
    bottom: 0;
    height: 4.5rem;
    width: 9rem;
  }
</style>

<div class="container">
  <div class="left half-circle">
    <div class="circle" />
  </div>
  <div class="right half-circle">
    <div class="circle" />
  </div>
</div>
