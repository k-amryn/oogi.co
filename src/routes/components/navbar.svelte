<script>
import Oogibox from "./oogibox.svelte";

</script>

<Oogibox px="10px">
  <div class="content">
    <img src="./oogi.png" alt="">
  </div>
</Oogibox>

<style>
  .content {
    width: 100%;
    display: flex;
    place-content: center;
  }
  img {
    width: 80px;
  }
</style>