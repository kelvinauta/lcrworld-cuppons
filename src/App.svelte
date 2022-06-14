<script>
 	let algo = "s5algo"
	import Menu from "./lib/Menu.svelte"
	import ListCards from "./lib/ListCards.svelte"
	import Text from "./lib/Text.svelte"
	import Footer from "./lib/Footer.svelte"
</script>

<main>
	<br/>
	<Text/>
	<br/>
	<ListCards/>
	<br/>
	<Footer/>
</main>

<style global>
	:global(body) {
		/* this will apply to <body> */
		margin: 0;
		font-family: sans-serif;
		background: #7e8bd3;
		color: #e6e7ed;

	}
	:global(h1,p) {
		/* this will apply to <body> */
		margin: 0;
		font-family: sans-serif;
	}

	
</style>
