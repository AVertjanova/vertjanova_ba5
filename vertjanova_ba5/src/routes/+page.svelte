<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<script>
    import Cell from '../lib/cell.svelte'
</script>


<h1 class="page">Count</h1>
<div class="boxes">
    <div class="cell">box 1</div>
    <div class="cell">box 2</div>
    <div class="cell">box 3</div>
    <div class="cell">box 4</div>
</div>

<style>
    .boxes{
    
        display: grid;
        justify-content: center;
    }
    
    .page{
        display: grid;
        justify-content: center;
    }
</style>