<div class="container">
  <div class="logo">
    <img style="width: 150px;" src="../logo_outline.png" alt="">
  </div>
  <div class="col 1">
    <span>About</span>
    <span>Roadmap</span>
    <span>FAQ</span>
  </div>
  <div class="col 2">
    <span>Community</span>
    <span>Coin</span>
    <span>NFT</span>
  </div>
  <div class="social">
    <img src="../social-discord.png" alt="discord link">
    <img src="../social-twitter.png" alt="twitter link">
  </div>

</div>

<style>
  .container {
    font-size: 16pt;
    box-sizing: border-box;
    padding: 20px;
    width: 100%;
    height: 150px;
    background: #fef2b6;
    display: grid;
    grid-template-columns: auto auto auto 1fr;
    gap: 25px;
  }
  .col {
    display: flex;
    flex-direction: column;
  }
  .social {
    justify-self: end;
  }
  .social img {
    filter: brightness(0);
  }
</style>