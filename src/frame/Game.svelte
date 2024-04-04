<script lang="ts">
	import Food from '../model/Food.svelte';


	let foodX=100;
	let foodY=200;

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
		}
</style>


<div class="center frame">
	<Food {foodX} {foodY}/>


</div>

