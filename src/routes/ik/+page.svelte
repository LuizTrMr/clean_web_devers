<script>
	let title = "Inverse Kinematics Demo";
	let description = ["A demo for the concept of Inverse Kinematics", "There is nothing to play here, just watch :)"];
</script>

<div class="container">
	<iframe src="Kinematics/Kinematics.html"></iframe>
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

	iframe {
		width : 100%;
		min-height: 80vh;
	}

	.info {
		padding: 20px;
		color: white;
	}
</style>
