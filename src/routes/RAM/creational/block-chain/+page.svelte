

<script>
  import { onMount } from "svelte";

  onMount(() => {
    var masonry2 = new MiniMasonry({
      container: document.querySelector('.block-chain'),
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
    <div class="WiFi">o---<a href="/RAM/creational/">isTrav</a>---o <span style="color: #888;">// creational patterns</span> <span style="float: right;"><span style="color: #888;">(<span style="color: #ffff00;">x</span>)>-&#123;<span style="color: #ff0000;">prototype</span>}=[</span><span class="title">block-chain</span><span style="color: #888;">]</span></div>
  </div>
</div>
<div class="console">
  <video class="log" controls autoplay muted loop>
    <source src="/RAM/creational/block-chain/BLOCK-CHAIN.mp4" type="video/mp4" />
  </video>
</div>
<div class="container block-chain">
  <div class="item" style=""><img src="/RAM/creational/block-chain/GENESIS.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/MINING.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/WALLET.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/FUNGIBILITY.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/LEDGER.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/PROOF_OF_WORK.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/SMART_CONTRACTS.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/DECENTRALIZATION.png" /></div>
  <div class="item" style=""><img src="/RAM/creational/block-chain/HASH.png" /></div>
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
