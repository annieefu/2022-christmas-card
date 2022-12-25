<script>
	import { getContext } from "svelte";
	import Demo from "$components/demo/Demo.svelte";
	import WIP from "$components/helpers/WIP.svelte";
	// import Footer from "$components/Footer.svelte";
	import Snow from '$components/card/Snow.svelte';

import Title from '$components/card/Title.svelte';

	// const copy = getContext("copy");
	// const data = getContext("data");
</script>
<!-- 
<WIP />
<Demo /> -->


<div class="whole=wrapper">
	<Snow />
	<Title />
</div>
<!-- <Footer /> -->


<style>
	body{
		height: 100vh !important;
		background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%) !important;
		overflow: hidden !important;
		filter: drop-shadow(0 0 10px white) !important;
	}
	
	.whole-wrapper{
		position: absolute;
		top: 0;
	}
	
	
	</style>