<script>
  import Cell from "../lib/cell.svelte";

  let boxGrid = $state(Array(4).fill("white"));
  let count = $derived(countBlack(boxGrid));

  function changeColor(i, color) {
    boxGrid[i] = boxGrid[i] === "white" ? "black" : "white";
  }

  function countBlack(boxGrid) {
    let total = 0;
    boxGrid.forEach((element) => {
      if (element === "black") {
        total += 1;
      }
    });
    return total;
  }
</script>

<h1 class="page">Count {count}</h1>
<div class="boxes">
  {#each boxGrid as cell, i}
    <Cell color={cell} index={i} switchColor={changeColor} />
  {/each}
</div>

<style>
  .boxes {
    display: grid;
    justify-content: center;
    grid-template-columns: repeat(2, 100px);
    gap: 0;
  }

  .page {
    display: grid;
    justify-content: center;
  }
</style>
