<div class="header">
  <div class="coins">
    <img class="coin l" style="right: 0" src="/coin.png" alt="coin">
    <img class="coin l" style="left: 180px; top: 160px" src="/coin.png" alt="coin">
    <img class="coin m" style="top: 50px; left: 20px" src="/coin.png" alt="coin">
    <img class="coin m" style="left: 210px; top: 50px" src="/coin.png" alt="coin">
    <img class="coin m" style="bottom: 20px; left: 60px" src="/coin.png" alt="coin">
    <img class="coin m" style="left: 360px; bottom: 100px" src="/coin.png" alt="coin">
    <img class="coin s" style="left: 110px; top: 120px" src="/coin.png" alt="coin">
  </div>
  <div class="apes">
    <img src="/coin_apes_left.png" alt="apes">
    <img src="/coin_apes_right.png" alt="apes">
  </div>
</div>

<style>
  .header {
    width: 100%;
    height: 800px;
    background-image: url(/banner.png);
    background-position: bottom;
    background-repeat: no-repeat;
    background-size: cover;

    display: grid;
    place-items: center;
    grid-template-rows: 1fr auto;
    position: relative;
  }

  .coins {
    margin-top: 150px;
    height: 400px;
    width: 500px;
    position: relative;
    /* background: rgba(200,120,120, 0.5); */
    z-index: 4;
    image-rendering: pixelated;
  }

  .coin {
    position: absolute;
  }

  .coin.l {
    width: 120px;
  }

  .coin.m {
    width: 90px;
  }

  .coin.s {
    width: 60px;
  }

  @keyframes example {

  }

  .apes {
    position:absolute;
    bottom: 0;
    
    width: 100%;
    max-width: 1200px;
    display: grid;
    grid-template-columns: auto auto;
    align-items: end;
    justify-content: space-between;
  }

  .apes img {
    width: 100%;
    max-width: 350px;
  }
</style>