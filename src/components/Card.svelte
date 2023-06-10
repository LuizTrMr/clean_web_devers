<script>
	import { page } from '$app/stores';
	import { goto } from '$app/navigation';
	export let title;
	export let description;
	export let thumbnail;
	export let url;

	let highlighted = false;
	function toggleHighlight() {
		highlighted = !highlighted;
	}
	
	function navigateTo(url) {
		goto(url);
	}
</script>


<div class="card"
	 on:mouseover={toggleHighlight}
	 on:mouseout={toggleHighlight}
	 on:blur={toggleHighlight}
	 on:focus={toggleHighlight}
	 on:click={navigateTo(url)}
	 on:keydown={navigateTo(url)}
	 style="background: {highlighted ? '#c6c4dd' : '#41404d'}"
>
	<img src={thumbnail} alt="Game Thumbnail"/>
	<h3 style="color: {highlighted ? 'black' : 'white'}">{title}</h3>
	<p  style="color: {highlighted ? 'black' : 'white'}">{description}</p>
</div>


<style>
	.card {
		width        : 400px;
		height       : 350px;
		border-radius: 10px;
		padding      : 10px;
		box-shadow   : 10px 10px 10px rgba(0,0,0,0.5);
		transition   : all 0.4s;
		cursor       : pointer;
	}

	.card:hover {
		transform : scale(1.05);
	}

	img {
		max-width : 100%;
	}
</style>
