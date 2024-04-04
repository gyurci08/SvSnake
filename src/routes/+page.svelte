<link href="https://fonts.googleapis.com/css2?family=Codystar:wght@300;400&display=swap" rel="stylesheet">

<script lang="ts">
	import Game from '../frame/Game.svelte';

	let score: number;
</script>

<style>

		.tx_center{
				text-align: center;
				font-family: "Codystar";
		}
</style>




<div class="">
	<h1 class="tx_center">Snake</h1>
	<h2 class="tx_center">Score: {score}</h2>
	<Game bind:score></Game>

</div>
