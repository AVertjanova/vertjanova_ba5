<script>
  import Cell from "../../lib/cell.svelte";
  function onboxclick(name) {
    console.log(name + "clicked");
  }
</script>

<p>
  Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
  documentation
</p>

<h1 class="page">Count</h1>
<div class="boxes">
  <Cell name="box 1"></Cell>
  <Cell name="box 2" {onboxclick}></Cell>
  <Cell name="box 3" {onboxclick}></Cell>
  <Cell name="box 4" {onboxclick}></Cell>
</div>

<style>
  .boxes {
    display: grid;
    justify-content: center;
  }

  .page {
    display: grid;
    justify-content: center;
  }
</style>
