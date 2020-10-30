<script>
  import { onMount } from "svelte";
  let mouseMove;
  let m = { x: 0, y: 0 };

  let windowWidth;

  function handleMousemove(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }

  $: isLeft = m.x <= windowWidth / 2 ? "start" : "end";
</script>

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

  .container.end:hover .circle {
    transform: translateX(10%);
    transition: transform 0.2s linear;
  }

  .container.end:hover .small {
    transform: translateX(35%);
  }
  .container.end:hover .big {
    transform: translateX(0);
  }

  .container.start:hover .circle {
    transform: translateX(-10%);
    transition: transform 0.2s linear;
  }

  .container.start:hover .small {
    transform: translateX(-35%);
  }
  .container.start:hover .big {
    transform: translateX(0);
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

<svelte:window bind:innerWidth={windowWidth} />

<div class="container {isLeft}" on:mousemove={handleMousemove}>
  <div class="big circle">
    <div class="circle">
      <div class="circle">
        <div class="small circle" />
      </div>
    </div>
  </div>
</div>
