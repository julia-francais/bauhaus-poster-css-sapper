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

  .one {
    position: absolute;
    background-color: #7eb6b5;
    opacity: 0.7;
    z-index: 1;
    overflow: hidden;
  }

  .two {
    position: absolute;
    transform: translateY(7rem);
    background-color: #c65233;
  }

  .circle:first-of-type::after {
    content: "";
    position: absolute;
    height: 10rem;
    width: 10rem;
    top: 7rem;
    opacity: 1;
    z-index: 2;
    background: #594484;
    border-radius: 100%;
  }
</style>

<div class="container">
  <div class="circle one" />
  <div class="circle two" />
</div>
