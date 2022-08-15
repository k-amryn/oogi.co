<script>
  import Navbar from './components/navbar.svelte';
  import Footer from './components/footer.svelte'

	import '../global.css';
</script>

<main>
  <Navbar />
  <slot />
  <div class="spacer"></div>
  <Footer />
</main>

<style>
  main {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  .spacer {
    flex: 1 0 auto;
  }
</style>