<script lang="ts">
	import Game from '../frame/Game.svelte';

	let score: number;
</script>

<style>
    .center{
        margin: auto;
        width: 90%;
        padding: 10px;
		}

		.tx_center{
				text-align: center;
		}
</style>




<div class="center">
	<h1 class="tx_center">Snake</h1>
	<Game bind:score></Game>
	<h2 class="tx_center">Score: {score}</h2>
</div>
