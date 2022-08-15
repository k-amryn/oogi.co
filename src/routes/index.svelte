<script>
  $: outerWidth = 0
  let scrollSrc = "scroll.png"
  let scrollLogo = "logo_graphic_outline.png"
  $: if (outerWidth < 640) {
    scrollSrc = "scroll_long.png"
    scrollLogo = "logo_outline.png"
  } else if (outerWidth < 740){
    scrollSrc = "scroll_long.png"
    scrollLogo = "logo_graphic_outline.png"
  } else if (outerWidth < 770){
    scrollSrc = "scroll_2.png"
    scrollLogo = "logo_outline.png"
  } else if (outerWidth < 860){
    scrollSrc = "scroll_2.png"
    scrollLogo = "logo_graphic_outline.png"
  } else {
    scrollSrc = "scroll.png"
    scrollLogo = "logo_graphic_outline.png"
  }
</script>

<svelte:window bind:outerWidth />

<main>
  <div class="header">
    <h1 style="margin-top: 100px; text-align: center">
      ascended from the jungle<br>
      hanging out on solana
    </h1>
    <img style="width: 200px" class="header-logo" src="oogi.png" alt="OOGI">
  </div>

  <div class="scroll-holder">
    <div class="scroll-inner">
      <img class="scroll-img" src={scrollSrc} alt="scroll">
      <div class="scroll-text">
        <p>
          It was a peaceful day in the jungle for the Oogi tribe of apes. The birds were chirping, and wind was flowing through the trees. The apes had no idea their lives were about to change forever.
        </p>
        <p>
          Suddenly, they noticed a strange whirring noise from the sky that became louder and louder, as if something was falling to the earth. Panicked and confused, the apes huddled behind a tree and hoped for the best. When the noise was almost unbearably loud...
        </p>
        <p>
          *WHAM*
        </p>
        <p>
          A large spherical pod crashed directly into their favorite eucalyptus tree. It was glowing purple from between its bolted segments, and emitting a distinct humming noise. As the apes were mourning the loss of their tree, the pod began opening up to reveal a mysterious alien technology.
        </p>
        <p>
          Sparing some of the details, the Oogi tribe soon found a new home on the Solana blockchain.
        </p>
      </div>
      <img class="scroll-logo" src={scrollLogo} alt="scroll logo">
    </div>
  </div>
</main>

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
  }
  .scroll-holder {
    box-sizing: border-box;
    padding: 50px 10px 50px 10px;
    width: 100%;
    display: flex;
    place-content: center;
  }
  .scroll-inner {
    position: relative;
    height: 100%;
    display: grid;
    justify-items: center;
  }
  .scroll-img {
    width: 100%;
    max-width: 900px;
    z-index: -2;
  }
  .scroll-text {
    position: absolute;
    box-sizing: border-box;
    font-size: 15pt;
    width: 100%;
    margin-top: 25%;
    padding: 0px 23% 0px 23%;
    max-width: 900px;
    z-index: 1;
  }
  .scroll-logo {
    position: absolute;
    bottom: 0;
    margin-bottom: 27%;
    width: 150px;
  }
  @media only screen and (max-width: 750px) {
    .scroll-logo {
    margin-bottom: 27%;
      width: 150px;
    }
  }
  @media only screen and (max-width: 720px) {
    .scroll-logo {
    margin-bottom: 33%;
      width: 200px;
    }
  }
  @media only screen and (max-width: 650px) {
    .scroll-logo {
      margin-bottom: 27%;
      width: 130px;
    }
  }
</style>