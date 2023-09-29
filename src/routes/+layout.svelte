<div class="Header" />

<slot />

<div class="box">
  <p style="color: white; text-align: center;">
    © Copyright 2023 by Zebadiah Lake
  </p>
</div>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
  }
  .box {
    width: auto;
    height: 56px;
    border-top: 0.5px solid black;
    background: #10071d;
    box-sizing: border-box;
    top: 1760px;
    position: relative;
  }
  .Header {
    width: auto;
    height: 56px;
    border-top: 0.5px solid black;
    background: #10071d;
    box-sizing: border-box;
    top: 0%;
    position: relative;
  }
</style>
