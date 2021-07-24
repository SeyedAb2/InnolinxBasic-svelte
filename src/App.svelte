
<script>
	import Nav from "./layout/Nav.svelte";
	import Footer from "./layout/Footer.svelte";
	import {fade , slide , scale , fly} from "svelte/transition";
	let y=0;
	$: console.log(y);	
</script>


<style global> 
	@import "/bootstrap.rtl.min.css";
	@import "/global.css";
</style>

<svelte:window bind:scrollY={y}/>

<Nav {y}/>

<Footer {y}/>
	
	







	
	
