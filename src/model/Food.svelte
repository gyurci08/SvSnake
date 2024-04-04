<script lang="ts">
	export let foodX: number;
	export let foodY: number;
</script>


<style>
    .dot {
        height: 25px;
        width: 25px;
        position: absolute;
        left: 0px;
        top: 0px;
        background-color: #bbb;
        border-radius: 50%;
    }
</style>

<span class="dot" style="left: {foodX}px; top: {foodY}px;"></span>
