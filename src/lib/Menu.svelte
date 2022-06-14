<script>
	import data from "../data.js"
	
	let count = 0
  const increment = () => {
    count += 1
  }
	let {menu, info} = data
</script>

<nav>
	<a href="/">
		<img src={info.logoUrl} width=35/>
	</a>
	<div class="menu">
		{#each menu as itemMenu}
			<a>
				{itemMenu.title}
			</a>
		{/each}
		
	</div>
</nav>

<style>
	nav {
background: #7e8bd3;
box-shadow:  5px 5px 8px #737ec0,
             -5px -5px 8px #8998e6;
		padding: 8px;
		display: flex;
		justify-content: space-between;
	}
	.menu {
		
		display: flex;
		justify-content: flex-end; 
		align-items: center;
	}
	.menu a {
		margin: 0 4px;
		cursor: pointer;
	}
</style>
