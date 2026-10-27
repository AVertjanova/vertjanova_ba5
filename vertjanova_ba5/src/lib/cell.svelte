<script>
  let { color, index, switchColor, onboxclick = undefined } = $props();
</script>

<button class="cell" onclick={() => switchColor(index, color)}>{color}</button>

<style>
  .cell {
    background-color: white;
    border: 1px solid gray;
    height: 100px;
    width: 100px;
    display: block;
  }
</style>
