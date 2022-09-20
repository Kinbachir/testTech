<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import Login from "./routes/Login.svelte";

  export let url = "";
</script>
<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }
</style>
<Router url="{url}">
  <div>
    <Route path="/">
<main>
<body>

<!-- Hero Section -->
<section class="text-gray-600 body-font">
  <div >
    <img style="width:100%" alt="hero" src="../src/assets/cover.jpg">
  </div>
  <div class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center">
	<div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 mb-10 md:mb-0">
	  <img class="object-cover object-center rounded" alt="hero" src="../src/assets/1.jpeg">
	</div>
	<div class="lg:flex-grow md:w-1/2 lg:pl-24 md:pl-16 flex flex-col md:items-start md:text-left items-center text-center">
	  <h1 class="title-font sm:text-4xl text-3xl mb-4 font-bold uppercase text-white">Test
		<br class="hidden lg:inline-block">1
	  </h1>
	  <p class="mb-8 leading-relaxed">Then create a first page under the "/" route; its layout should resemble the image below..</p>
	  <div class="flex justify-center">
		<Link to="sign-in" class="btn btn-primary inline-flex text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg" >Login</Link>
	  </div>
	</div>
  </div>
  <div class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center">
	<div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 mb-10 md:mb-0">
	  <img class="object-cover object-center rounded" alt="hero" src="../src/assets/1.jpeg">
	</div>
	<div class="lg:flex-grow md:w-1/2 lg:pl-24 md:pl-16 flex flex-col md:items-start md:text-left items-center text-center">
	  <h1 class="title-font sm:text-4xl text-3xl mb-4 font-bold uppercase text-white">Test
		<br class="hidden lg:inline-block">1
	  </h1>
	  <p class="mb-8 leading-relaxed">Then create a first page under the "/" route; its layout should resemble the image below..</p>
	  <div class="flex justify-center">
		<Link to="sign-in" class="btn btn-primary inline-flex text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg">Login</Link>
	  </div>
	</div>
  </div>
</section>
<!-- End Hero Section -->

</body>
</main></Route>
    <Route path="sign-in" component="{Login}" />
  </div>
</Router>
