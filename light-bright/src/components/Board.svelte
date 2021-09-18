<script>
    import Tile from './Tile.svelte'
</script>

<div class="container">
    <div class="buttons">
        <button>Remove previous</button>
        <button>clear</button>
    </div>
    <div class="board">
        <Tile/>
    </div>
</div>

<style >
    .buttons {
        margin: 10px 0;
    }
    .board {
        width: 500px;
        height: 500px; 
        /* background: hsl(0, 0%, 50%); */
        background: hsl(0, 0%, 31%);

        display: grid;
        grid-template-rows: repeat(10, 1fr);
        grid-template-columns: repeat(10,1fr);
    }
</style>
