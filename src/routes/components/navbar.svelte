<script>
import Oogibox from "./oogibox.svelte";
import { page } from '$app/stores';
</script>

<div id="header">
  <div id="header-inner">
    <Oogibox px="10px">
      <div class="content">
        <a class="logo-img" href="/">
          <img src="/logo.png" alt="logo" style="width: 70px">
        </a>
        <span class="home" class:active={$page.routeId == ''}>
          <a href="/">Home</a>
        </span>
        <span class:active={$page.routeId == 'community'}>
          <a href="/community">Community</a>
        </span>
        <span class:active={$page.routeId == 'coin'}>
          <a href="/coin">Coin</a>
        </span>
        <span class:active={$page.routeId == 'nft'}>
          <a href="/nft">NFT</a>
        </span>
      </div>
    </Oogibox>
  </div>
</div>

<style>
  * {
    box-sizing: border-box;
  }
  .active {
    position: relative;

  }
  .active::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: -5px;
    width: calc(100% + 10px);
    height: 3px;
    background: black;
  }
  #header {
    position:fixed;
    width: 100%;
    padding: 50px 20px 0px 20px;
    display: flex;
    justify-content: center;
    pointer-events: none;
    z-index: 100;
  }
  #header-inner {
    width: 100%;
    max-width: 1200px;
    height: 100px;
    pointer-events: all;
  }
  .content {
    width: 100%;
    padding: 0px 100px;
    display: flex;
    place-content: center;
    place-items: center;
    position: relative;
    justify-content: space-around;
  }
  .logo-img {
    position: absolute;
    left: 20px;
    padding-top: 5px;
  }
  @media only screen and (max-width: 740px) {
    .home {
      display: none;
    }
  }
  a {
    text-decoration: none;
    color: black;
  }
</style>