
<script>
  import { onMount } from "svelte";

  onMount(() => {
    var masonry2 = new MiniMasonry({
      container: document.querySelector('.behavioral'),
      surroundingGutter: true,
      gutterX: 40,
      gutterY: 40,
      baseWidth: 400
    });
  })
</script>

<br />
<br />
<div style="max-width: 1000px; margin: 0 auto;">
  <div class="router">
    <div class="WiFi">o---<a href="/">isTrav</a>---o <span style="color: #888;">// behavioral patterns</span> <span style="float: right; color: #888;"><span style="color: #ffff00;">o---(</span><span style="color: #ff0000;">RAM</span><span style="color: #ffff00;">)</span></span></div>
  </div>
</div>
<br />
<br />
<div class="container behavioral">
  <div class="item" style="border: 1px solid #ff0000;">
    <video class="log" controls autoplay muted loop>
      <source src="./block-chain/BLOCK-CHAIN.mp4" type="video/mp4" />
    </video>
    <hr style="border-color: #ff0000; margin: 0;">
    <span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">prototype</span>}=[</span><a href="./block-chain/" class="title">block-chain</a><span style="color: #888;">]</span>
  </div>
  <div class="item" style="border: 1px solid #ff0000;">
    <video class="log" controls autoplay muted loop>
      <source src="./semiconductor/SEMICONDUCTOR.mp4" type="video/mp4" />
    </video>
    <hr style="border-color: #ff0000; margin: 0;">
    <span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">factory method</span>}=[</span><a href="./machine/" class="title">machine</a><span style="color: #888;">]</span>
  </div>
  <div class="item" style="border: 1px solid #ff0000;">
    <video class="log" controls autoplay muted loop>
      <source src="./semiconductor/SEMICONDUCTOR.mp4" type="video/mp4" />
    </video>
    <hr style="border-color: #ff0000; margin: 0;">
    <span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">abstract factory</span>}=[</span><a href="./semiconductor/" class="title">semiconductor</a><span style="color: #888;">]</span>
  </div>
  <div class="item" style="border: 1px solid #ff0000;">
    <video class="log" controls autoplay muted loop>
      <source src="./shop/SHOP.mp4" type="video/mp4" />
    </video>
    <hr style="border-color: #ff0000; margin: 0;">
    <span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">builder</span>}=[</span><a href="./shop/" class="title">shop</a><span style="color: #888;">]</span>
  </div>
  <div class="item" style="border: 1px solid #ff0000;">
    <video class="log" controls autoplay muted loop>
      <source src="../../shredder.mp4" type="video/mp4" />
    </video>
    <hr style="border-color: #ff0000; margin: 0;">
    <span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">singleton</span>}=[</span><a href="./storyboard/" class="title">storyboard</a><span style="color: #888;">]</span>
  </div>
</div>
<br />
<br />