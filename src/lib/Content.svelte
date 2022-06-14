<script>
		export let title, description, banner, link, logo; 
	import Button from "./Button.svelte"
</script>
<div class="Content">

	
	<div class="contentHead"> 
	<img src={logo} height=35/>
		<h1>{title}</h1>
	</div>
	<div class="banner">
		<img src={banner}/>
	</div>
	<div class="contentBody">
		{description}
	</div>
	<div class="contentAction">
			<a href={link}>
		<Button>
				Go Link
		</Button>
			</a>
	</div>
</div>

<style>
	.Content{
		font-family: sans-serif;
		background: #7e8bd3;
		color: #e6e7ed;
	}

	.contentHead{
		display: flex;
		margin: 16px 0;
	}
	.banner img{
		width: 100%;
	}
	.contentBody{
		margin: 16px 0;
	}
	.contentAction{
		width: 100%;
		display: flex;
		justify-content: center;
		
	}
</style>