<style>
  .container {
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .circle {
    height: 10rem;
    width: 10rem;
    border-radius: 50%;
    background-color: #ef1c21;
  }

  .half-circle {
    height: 10rem;
    width: 5rem;
    margin-left: 5rem;
    border-radius: 0 5rem 5rem 0;
    background-color: #f4be17;
  }
  .rectangle {
    position: absolute;
    background-color: black;
    height: 10rem;
    width: 5rem;
  }
  .rect-circle {
    position: absolute;
    background-color: #005baa;
    border-radius: 0 5rem 0 0;
    height: 10rem;
    width: 5rem;
  }
</style>

<div class="container">
  <div class="container-one">
    <div class="rect-circle" />
    <div class="half-circle" />
  </div>
  <div class="container-second">
    <div class="rectangle" />
    <div class="circle" />
  </div>
</div>
