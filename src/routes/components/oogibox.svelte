<script>
  export let px = "10px"
  export let bgMain = "#FEF2B6"
  export let bgAccent = "#F9E676"
</script>

<div id="nav" style="--px-size: {px}; --bg-main: {bgMain}; --bg-accent: {bgAccent}">
  <div class="squares">
    <div class="r one">
      <div class="square outer"></div>
      <div class="square inner"></div>
      <div class="space"></div>
      <div class="square inner"></div>
      <div class="square outer"></div>
    </div>

    <div class="vspace"></div>

    <div class="r two">
      <div class="square outer"></div>
      <div class="square inner"></div>
      <div class="space"></div>
      <div class="square inner"></div>
      <div class="square outer"></div>
    </div>
  </div>

  <div id="nav-inner">
    <slot />
  </div>
</div>

<style>
  * {
    box-sizing: border-box;
  }
  #nav {
    height: 100%;
    width: 100%;
    background: var(--bg-accent);
    position: relative;
    padding: var(--px-size) calc(var(--px-size)*3) var(--px-size) calc(var(--px-size)*3);
  }
  #nav-inner {
    height: 100%;
    width: 100%;
    background: var(--bg-main);
    display: flex;
    align-items: center;
  }
  .squares {
    pointer-events: none;
    position: absolute;
    width: 100%;
    height: 100%;
    padding: var(--px-size) 0px var(--px-size) 0px;
    top: 0;
    left: 0;
    display: grid;
    grid-template-rows: calc(var(--px-size)) auto calc(var(--px-size));
  }
  .r {
    display: grid;
    grid-template-columns: auto auto 1fr auto auto;
    
  }
  .square {
    width: var(--px-size);
    height: var(--px-size);
  }
  .square.outer {
    background: var(--bg-main);
    margin-left: var(--px-size);
    margin-right: var(--px-size);
  }
  .square.inner {
    background: var(--bg-accent);
  }
</style>

