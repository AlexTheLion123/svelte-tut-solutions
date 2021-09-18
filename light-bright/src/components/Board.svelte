<script>
    import Tile from './Tile.svelte'
    import Button from './Button.svelte'
    let background = 'rgb(46, 46, 46)';

    const clear = () => {
        background=''
        background = 'rgb(46, 46, 46)'
    }

</script>

<div class="container">
    <Button on:clear={clear}/>
    <div class="board">
        {#each Array(100) as _, i}
        <Tile background={background}/>
        {/each}
    </div>
</div>

<style >
    
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
