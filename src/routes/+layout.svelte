<script>
  import githubIcon from "/static/github.png";
  import linkedInIcon from "/static/linkedin.png";
</script>

<div class="header">
  <div
    class="header-image-link"
    style="background: url({githubIcon}) no-repeat center"
  />
  <div
    class="header-image-link"
    style="background: url({linkedInIcon}) no-repeat center"
  />
  <div class="header-image-link" style="background-color:aqua;" />
</div>

<div
  style="background-image: url(../images/background_lightmode.png) no-repeat center center fixed;"
>
  <slot />
</div>

<div class="footer">
  <p style="margin: auto; color: white; text-align: center;">
    © Copyright 2023 by Zebadiah Lake
  </p>
</div>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
  }
  .footer {
    display: flex;
    flex-shrink: 0;
    width: auto;
    height: 56px;
    border-top: 1px solid black;
    background: #10071d;
    box-sizing: border-box;
  }
  .header {
    width: auto;
    height: 56px;
    border-top: 1px solid black;
    background: #10071d;
    display: flex;
    justify-content: right;
  }
  .header-image-link {
    width: 38px;
    height: 39px;
    border-radius: 384px;
    margin-bottom: 8px;
    margin-top: 8px;
    margin-right: 27px;
    flex-shrink: 0;
  }
</style>
