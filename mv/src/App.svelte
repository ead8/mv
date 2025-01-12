<script>
  import { Router, Link, Route } from "svelte-routing";
  import { wrap } from "svelte-spa-router/wrap";
  
  // Import your pages
  import Home from "./routes/+page.svelte";
  import About from "./routes/about/+page.svelte";
  import Contact from "./routes/contactus/+page.svelte";
  import Portfolio from "./routes/portfolio/+page.svelte";
  import PortfolioDetails from "./routes/portfolio-details/+page.svelte";
  import Service from "./routes/service/+page.svelte";
	import Navbar from "./lib/components/Navbar.svelte";
	import Footer from "./lib/components/Footer.svelte";

  // Get the base URL for routing
  export let url = "";
</script>

<Router {url}>
  
  <main class="flex min-h-screen flex-col mx-auto overflow-hidden">
    <Navbar/>
    <Route path="/" component={Home} />
    <Route path="/about" component={About} />
    <Route path="/contact" component={Contact} />
    <Route path="/portfolio" component={Portfolio} />
    <Route path="/portfolio-details/:id" component={PortfolioDetails} />
    <Route path="/service" component={Service} />
    <Footer/>
  </main>

</Router>