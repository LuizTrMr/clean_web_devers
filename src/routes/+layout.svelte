<script>
</script>


<div class="jumbotron">
	<h1><a href="/">Gaming Hub</a></h1>
	<h3>Follow my programming adventures at <a href="https://github.com/LuizTrMr">LuizTrMr</a></h3>
</div>

<section>
	<slot />
</section>


<style>

	:global(body) {
		background-color: #8A624D;
		margin: 0;
	}

	.jumbotron {
		background-color: black;
		color: white;
		padding: 40px;
		text-align: center;
	}

	section {
		margin: 40px;
		display: flex;
		justify-content: center;
		align-items: center;}

	a {
		color:inherit;
	}

</style>
