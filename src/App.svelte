<script>
	import { Router, Link, Route } from "svelte-routing";
	import about from "./routes/about.svelte";
	import contact from "./routes/contact.svelte";
	export let url = "";
</script>

<style global> 
	@import "/bootstrap.rtl.min.css";
	@import "/global.css";
</style>

<h1 class="bg-success">سلام دوست من به اینولینکس خوش آمدید</h1>
<Router url="{url}">
	<nav>
	  <Link to="/">Home</Link>
	  <Link to="about">About</Link>
	  <Link to="contact">Contact</Link>
	</nav>
	<div>
	  <Route path="contact" component="{contact}" />
	  <Route path="about" component="{about}" />
	  <Route path="/" />
	</div>
  </Router>