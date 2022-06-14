<script>
	import Button from "./Button.svelte"
	
	import Content from "./Content.svelte"
	import { getContext } from 'svelte';	
 const { open } = getContext('simple-modal');
	export let title, description, banner, link, logo; 
  const showSurprise = () => open(Content, { title, description, banner, link, logo});
	
</script>
<div class="Card">
	<div>
		
	<img class="banner" src={banner}/>
	<div class="cardContent">
		<div>
			<h1>
				{title}
			</h1>
		 	<img class="logo" src={logo} width=35 height=35/>
		</div>
	</div>
	</div>
	<div class="cardAction">
			<Button onclick={showSurprise}>
				<a>More information</a>
			</Button>
	</div>
</div>

<style>
	.Card{
		width: 270px;
background: #7e8bd3;
box-shadow:  31px 31px 75px #717dbe,
             -31px -31px 75px #8b99e8;
		border-radius: 8px;

		margin: 16px 8px;
		height: auto;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		align-items: center;
	}
	.Card .banner{
		border-radius: 8px 8px 0 0;
		width: 270px;
	}
	
	.Card .cardContent{
		padding: 16px;
	}
	.cardContent div{
		display: flex;
		justify-content: space-between;
	}

	.Card h1{
		margin-bottom: 4px;
	}
	.Card p{
		margin-bottom: 4px;
	}
	.Card a{
		
	}
	.cardAction{
			padding-bottom: 16px;
	}
	button{
		
	}

	
</style>