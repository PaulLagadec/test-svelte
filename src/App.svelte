<script>
  // on importe le routeur
  import Router from "svelte-spa-router";

  // on importe les pages
  import Home from "./lib/pages/Home.svelte";
  import Portfolio from "./lib/pages/Portfolio.svelte";
  import Contact from "./lib/pages/Contact.svelte";
  import NotFound from "./lib/pages/Home.svelte";
  import Header from "./lib/components/Header.svelte";
  import Footer from "./lib/components/Footer.svelte";

  // variable qui contient les routes
  const routes = {
    "/": Home,
    "/portfolio": Portfolio,
    "/contact": Contact,
    "*": Home, 
  };
  
</script>
<!-- utilisation du routeur pour afficher les pages.On lui passe la liste des components. -->
<div class="container">
  <Header />
  <Router {routes} />
  <Footer />
</div>



