<script>
	import Card       from "../components/Card.svelte";
	import kinematics from '$lib/images/kinematics.png';
</script>


<div class="container">
	<Card title="Inverse Kinematics" description="Inverse Kinematics Demo built with Godot 3.0" thumbnail={kinematics} url="/ik"/>
	<Card title="Kinematics2" description="Inverse Kinematics Demo2" thumbnail={kinematics} url="/ik"/>
	<Card title="Inverse Kinematics" description="Inverse Kinematics Demo built with Godot 3.0" thumbnail={kinematics} url="/ik"/>
	<Card title="Kinematics2" description="Inverse Kinematics Demo2" thumbnail={kinematics} url="/ik"/>
</div>


<style>

	.container {
		display: grid;
		grid-template-columns: auto auto auto; /* 3 columns before it starts wrapping */
		grid-gap: 20px; /* Optional spacing between items */
	}

</style>
