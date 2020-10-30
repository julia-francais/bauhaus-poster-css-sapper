<script>
  import Nav from "../components/Nav.svelte";
</script>

<style>
  main {
    position: relative;
    width: 100%;
    height: 100%;
    background-color: #ede1c0;
    padding: 0;
    margin: 1.5rem auto 0;
    box-sizing: border-box;
  }
</style>

<Nav />

<main>
  <slot />
</main>
