<script>
	let title = "Inverse Kinematics Demo";
	let description = ["A demo for the concept of Inverse Kinematics", "There is nothing to play here, just watch :)"];
</script>

<div class="container">
	<div class="wrapper">
		<iframe title="Game" src="Kinematics/Kinematics.html"></iframe>
	</div>
	<div class="info">
		<h1>{title}</h1>
		{#each description as paragraph}
			<p>{paragraph}</p>
		{/each}
	</div>
</div>

<style>
	.container {
		width: 100%;
		background-color: #713827;
	}

	.wrapper {
		width : 100%;
		height: 80vh;
		margin: 0 auto;
		position: relative;
		background-position: 50% 50%;
	}

	iframe {
		height: 0;
		width: 0;
		border: 0;
		box-sizing: border-box;
		max-height: 100%;
		max-width: 100%;
		min-height: 100%;
		min-width: 100%;
	}

	.info {
		padding: 20px;
		color: white;
	}
</style>
