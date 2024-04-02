<script>
  import Navbar from '../components/Navbar.svelte';
  import Footer from '../components/Footer.svelte';
  import '../app.css';
</script>

<nav>
   <Navbar/>
</nav>

<main>
  <slot/>
</main>

<footer>
   <Footer/>
</footer>
