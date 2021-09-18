<script>
	export let name;
	import Board from './components/Board.svelte';
</script>

<h1>Light-Bright</h1>
<Board/>

<style> 
	:global(body) {
		background: hsl(0, 0%, 20%);
		color: hsl(0, 0%, 98%);
		padding: 10px;
	}
</style>


