<script>
  import { onMount } from "svelte";

  onMount(() => {
    var masonry2 = new MiniMasonry({
      container: document.querySelector('.semiconductor'),
      surroundingGutter: true,
      gutterX: 40,
      gutterY: 40,
      baseWidth: 400
    });
  })
</script>

<br />
<br />
<div style="width: 100%; max-width: 1000px; margin: 0 auto;">
  <div class="router">
    <div class="WiFi">o---<a href="/RAM/creational/">isTrav</a>---o <span style="color: #888;">// creational patterns</span> <span style="float: right;"><span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">abstract factory</span>}=[</span><span class="title">semiconductor</span><span style="color: #888;">]</span></div>
  </div>
</div>
<div class="console">
  <video class="log" controls autoplay muted loop>
    <source src="/RAM/creational/semiconductor/SEMICONDUCTOR.mp4" type="video/mp4" />
  </video>
</div>
<div class="container semiconductor">
  <div class="item" style=""><img src="/RAM/creational/semiconductor/STORAGE.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/semiconductor/COMPUTE.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/semiconductor/RADIATOR.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/semiconductor/DRY.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/semiconductor/WET.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/semiconductor/UPS.png" /></div>
</div>
<br />
<br />

<style>
  .console {
    margin: 2.5em;
    border: 0.5em solid #000;
    overflow: hidden;
    background: #000;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 1);
  }
  .console .log {
    width: 100%;
  }
</style>