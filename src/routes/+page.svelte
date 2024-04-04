<script>
	import Game from '../frame/Game.svelte';


	let score=0;
</script>

<style>
    .center{
        margin: auto;
        width: 90%;
        border: 3px solid black;
        padding: 10px;
		}

		.tx_center{
				text-align: center;
		}
</style>




<div class="center">
	<h1 class="tx_center">Snake</h1>
	<Game></Game>
	<h2 class="tx_center">Score: {score}</h2>
</div>
