<script>
	export let onclick;
	let color = "black"
</script>
<button on:click ={onclick} >

	<slot></slot>
</button>

<style>
	button{
		margin-top: 4px;
		cursor: pointer;
		color: #e6e7ed;
		border-radius: 4px;
		text-transform: uppercase;
		padding: 8px 10px;
		font-size: 1.2em;
		transition: 0.2s;
	
		background: linear-gradient(145deg, #8795e2, #717dbe);
		box-shadow:  5px 5px 8px #646ea7,
	             -5px -5px 8px #98a8ff;
		border:none;
	}
	button:hover{
		background: #7e8bd3;
		box-shadow: inset 5px 5px 8px #646ea7,
		            inset -5px -5px 8px #98a8ff;

	}
	button:active{
		transform: scale(0.95)
	}
</style>