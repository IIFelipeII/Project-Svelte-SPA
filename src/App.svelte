<script lang="ts">
			import { Router, Link, Route } from "svelte-routing";
			import Home from './views/Home.svelte'
			import Map from './views/Map.svelte'
			import Start from './views/Start.svelte' 
			import Write from './views/Write.svelte'
			import Nav from './Components/Navbar.svelte'
		
			

</script>

<main>

<!-- <Start></Start> -->
<div>
	<Router>
		<!-- <nav>
			<Link to="/">Start</Link>
			<Link to="/Home">Home</Link>
			<Link to="/Maps">Maps</Link>

		</nav> -->


			<!-- <Nav></Nav> -->

		<Route path="/">
			<Start></Start>
		</Route>

		<Route path="/Write">
			<Write></Write>
		</Route>

		<Route path="/Home">
			<Home></Home>
		</Route>
		<Route path="/Maps">
			<Map></Map>
		</Route>
	</Router>
</div>
</main>
<style>

  :root {
    font-family: 'Nunito', sans-serif;
  }
 
  main {
	min-height: 100vh;
    color: white;
    padding: .8em;
	 background: rgb(78,55,158);
    background: linear-gradient(167deg, rgba(78,55,158,1) 0%, rgba(136,61,242,1) 29%, rgba(215,98,217,1) 100%);
 	 background-repeat: no-repeat;
	 background-size: cover;
    
  }
  
</style>
