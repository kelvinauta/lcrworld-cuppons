<script>

	import Card from "./Card.svelte"
	import data from "../data.js"
	import Modal from 'svelte-simple-modal';
	const {cards} = data
</script>
<div>
	{#each cards as card}
	<Modal styleWindow={{background: "#7e8bd3"}}>
		
		<Card {...card}/>
	</Modal>
	{/each}
	
</div>

<style>
	div{
		display: flex;
		justify-content: space-around;
		flex-wrap: wrap;
	}
</style>