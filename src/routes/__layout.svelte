<script>
  import Navbar from './components/navbar.svelte';
  import Footer from './components/footer.svelte'

	import '../global.css';
</script>

<main>
  <Navbar />
  <slot />
  <Footer />
</main>

<style>
</style>