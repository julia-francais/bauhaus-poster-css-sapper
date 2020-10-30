<script>
</script>

<style>
  .container {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
  }
  .circle {
    height: 10rem;
    width: 10rem;
    border-radius: 50%;
  }

  .circle:first-of-type::after {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    right: -60px;
    background: #fff;
    border-radius: 101px;
  }

  .circle + .circle::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: -60px;
    background: #fff;
    border-radius: 101px;
  }

  .one {
    position: absolute;
    background-color: #7eb6b5;
    transform: translateY(62px);
    opacity: 0.7;
    z-index: 1;
  }

  .two {
    position: absolute;
    transform: translateX(25px);
    background-color: #c65233;
  }
</style>

<div class="container">
  <div class="circle one" />
  <div class="circle two" />
</div>
