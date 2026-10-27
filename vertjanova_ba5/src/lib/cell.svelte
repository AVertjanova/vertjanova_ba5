<script>
  let { color, index, switchColor, onboxclick = undefined } = $props();
</script>

<button
  class="whitecell"
  style:background-color={color}
  onclick={() => switchColor(index, color)}>{color}</button
>

<style>
  button {
    background-color: white;
    border: 1px solid gray;
    height: 100px;
    width: 100px;
    display: block;
  }

  .blackcell {
    background-color: black;
    border: 1px solid gray;
    height: 100px;
    width: 100px;
    display: block;
  }
</style>
