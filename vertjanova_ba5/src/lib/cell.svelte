<script>
  let { name, onboxclick = undefined } = $props();
</script>

<div class="cell" onclick={onboxclick(name)}>{name}</div>

<h1></h1>

<style>
  .cell {
    background-color: white;
    border: 1px solid gray;
    height: 100px;
    width: 100px;
  }
</style>
