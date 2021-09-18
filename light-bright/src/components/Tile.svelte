<script>
    export let background;
    const randomColor = () => {
        const r = Math.floor(Math.random()*16777215).toString(16);
        background = `#${r}`;
    }

</script>

<div class="tile" on:click={randomColor} style="background: {background}"></div>

<style>
    .tile{
        width: 100%;
        height: 100%;
        border-radius: 100%;
        background: rgb(46, 46, 46);
    }
    
</style>