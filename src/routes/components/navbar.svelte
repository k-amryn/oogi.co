<script>
import Oogibox from "./oogibox.svelte";

</script>

<div id="header">
  <div id="header-inner">
    <Oogibox px="10px">
      <div class="content">
        <img src="../logo.png" alt="">
      </div>
    </Oogibox>
  </div>
</div>

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
  .content {
    width: 100%;
    display: flex;
    place-content: center;
  }
  img {
    width: 80px;
  }
</style>