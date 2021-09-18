<script>
    import { createEventDispatcher } from 'svelte';
    const dispatch = createEventDispatcher();

    const clear = () => {
        dispatch('clear')
    }

    const removePrev = () => {

    }
</script>

<div class="buttons">
    <button on:click={removePrev}>Remove previous</button>
    <button on:click={clear}>clear</button>
</div>

<style>
    .buttons {
        margin: 10px 0;
    }
</style>