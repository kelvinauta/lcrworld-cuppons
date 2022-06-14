<script>
	import data from "../data.js"
	const {info} = data
</script>
<div>
	
	<p>
		{info.signature}{` `}
		<a href={info.privacyPolice}>Privacy Policy</a>
	</p>
	
</div>

<style>
	div{
		padding: 8px;
		background: #7e8bd3;
		box-shadow:  31px 31px 75px #717dbe,
             -31px -31px 75px #8b99e8;
		text-align: center;
	}
</style>