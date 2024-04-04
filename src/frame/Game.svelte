<script lang="ts">
	import Food from '../model/Food.svelte';
	import Snake from '../model/Snake.svelte';


	let foodX=100;
	let foodY=200;

	let snakeBodies=[
		{
			left: 100,
			top: 0
		},
		{
			left: 50,
			top: 0
		},
		{
			left: 0,
			top: 0
		}
	]

	 let direction: string = "right"


	function onKeyPress(e: KeyboardEvent){
			//console.log(e.key)
			const newDirection = setDirectionFromKey(e.key);
			if(newDirection){
				direction = newDirection;
			}

	}

	function setDirectionFromKey(key: string){
		if (key === "ArrowDown"){
			return "down"
		}
		else
			if (key === "ArrowUp"){
				return "up"
		}
			else
				if (key === "ArrowLeft"){
					return "left"
			}
				else
				if (key === "ArrowRight"){
					return "right"
				}
	}





</script>

<style>
    .center{
        margin: auto;
        border: 3px solid black;
        padding: 10px;
    }

		.frame{
				width: 500px;
        height: 500px;
				position: relative;
				z-index: 0;
		}
</style>


<div class="center frame">
	<Food {foodX} {foodY}/>
	<Snake {snakeBodies} {direction}/>
</div>

<svelte:window on:keydown={onKeyPress} />