<script>
  import Navbar from './components/navbar.svelte';

	import '../global.css';
</script>

<main>
  <div id="header">
    <div id="header-inner">
      <Navbar />
    </div>
  </div>
  <slot />
</main>

<style>
  * {
    box-sizing: border-box;
  }
  #header {
    position:fixed;
    width: 100%;
    display: flex;
    height: 150px;
    padding: 50px 20px 0px 20px;
    display: flex;
    justify-content: center;
  }
  #header-inner {
    width: 100%;
    max-width: 1200px;
  }
</style>