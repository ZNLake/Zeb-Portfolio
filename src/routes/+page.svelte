<script>
  import Carousel from "svelte-carousel";
  import backgroundWhite from "/static/background_lightmode.png";
  import backgroundBlack from "/static/background_darkmode.png";
  import rustIcon from "/static/rust.png";
  import cIcon from "/static/c-lang.png";
  import cPlusIcon from "/static/c-plusplus.png";
  import cSharpIcon from "/static/c-sharp.png";
  import javaIcon from "/static/java.png";
  import pythonIcon from "/static/python.png";
  import svelteIcon from "/static/svelte.png";
  import sqlIcon from "/static/sql.png";
  import htmlIcon from "/static/html.png";
  import cssIcon from "/static/css.png";
  import jsIcon from "/static/js.png";
  import agileIcon from "/static/agile.png";
  import flexibleIcon from "/static/flexible.png";
  import fullstackIcon from "/static/fullstack.png";
  import headshot from "/static/headshot.png";
  import mongodbIcon from "/static/mongodb.png";
  import sendIcon from "/static/send.png";
  let backgroundSrc = backgroundWhite;
  let icons = [
    rustIcon,
    cIcon,
    cPlusIcon,
    cSharpIcon,
    javaIcon,
    pythonIcon,
    svelteIcon,
    sqlIcon,
    mongodbIcon,
    cssIcon,
    htmlIcon,
    jsIcon,
  ];
</script>

<div
  class="wrapper"
  style="background:url({backgroundSrc}) no-repeat center; background-size: cover;"
>
  <div class="section-two">
    <div class="section-two-subgrid">
      <div style="grid-column: 1;" />
      <div style="grid-column: 2; justify-content: center;">
        <div class="section-two-introduction">
          <span class="introduction-part-one"
            >Hi, my name is Zebadiah Lake!</span
          >
          <span class="introduction-part-two"
            >Welcome to my Portfolio! I am a full-time Computer Science student
            based in Ontario, Canada excited to work on thrilling projects and
            technology!
          </span>
        </div>
        <div class="skill-bubble">
          <div
            class="skill-image"
            style="margin-left: 6px; background: url({fullstackIcon}) no-repeat center"
          />
          <span class="skill-name" style="margin-left: 8px;">Full Stack</span>
          <span
            class="skill-description"
            style="width: 176px; height: 29px; margin-top: 15px; margin-bottom: 16px; margin-right: 24px; margin-left: 11px;"
            >I do full stack software development!
          </span>
        </div>
        <div class="skill-bubble">
          <div
            class="skill-image"
            style="margin-left: 6px; background: url({flexibleIcon}) no-repeat center"
          />
          <span class="skill-name" style="margin-left: 8px; width: 75px;"
            >Flexible</span
          >
          <span class="skill-description" style="width: 221px; height: 60px;"
            >I am capable in working with both<br />upcoming and industry
            standard software</span
          >
        </div>
        <div class="skill-bubble">
          <div
            class="skill-image"
            style="margin-left: 6px; background: url({agileIcon}) no-repeat center"
          />
          <span class="skill-name" style="margin-left: 8px;">Agile</span>
          <span
            class="skill-description"
            style=" width: 176px; height: 29px; margin-top: 15px; margin-bottom: 16px; margin-right: 24px; margin-left: 11px;"
            >I do full stack software development!</span
          >
        </div>
      </div>
      <div style="grid-column: 3; display: flex; justify-content: right;">
        <div
          class="section-two-picture"
          style="background image: url({headshot})"
        />
      </div>
      <div style="grid-column: 4;" />
    </div>
  </div>
  <div class="section-three">
    <div class="section-three-line" />
    <p class="section-three-experience">Experience</p>
    <p class="section-three-subtitle">
      Take a look below at some of the projects I have completed!
    </p>
  </div>
  <div class="section-four">
    <div class="tile-row">
      <div class="top-experience-tile" />
      <div class="top-experience-tile" />
      <div class="top-experience-tile" />
    </div>
    <div class="tile-row">
      <div class="bottom-experience-tile" />
      <div class="bottom-experience-tile" />
      <div class="bottom-experience-tile" />
    </div>
  </div>
  <div class="section-five">
    <div
      style="display:flex; max-width:800px; margin: auto; margin-top: 5%; margin-bottom: 5%"
    >
      <Carousel
        autoplay
        duration={2000}
        autoplayDuration={0}
        particlesToShow={5}
        dots={false}
        timingFunction="linear"
        arrows={false}
        swiping={false}
      >
        {#each icons as icon}
          <div
            class="lower-icons"
            style="background: url({icon}) no-repeat center"
          />
        {/each}
      </Carousel>
    </div>
  </div>
  <div class="section-six">
    <div class="section-six-line" />
    <p class="working-with-me">
      Interested in working with me? Or got feedback?
    </p>
    <div class="contact-me">
      <span class="contact-me-text" style="color: black; text-align: center;"
        >Contact Me!</span
      >
      <div class="section-six-send" style="background: url({sendIcon})" />
    </div>
  </div>
</div>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
  }
  .corner-graphic {
    position: relative;
    top: 22.6vh;
    left: 82.49vw;
    width: 195px;
    height: 219px;
  }
  .wrapper {
    display: grid;
    grid-auto-rows: minmax(100px, auto);
    margin: 0;
    padding: 0;
  }

  .section-two {
    grid-row: 2;
    margin-top: 140px;
    margin-bottom: 140px;
  }
  .section-two-subgrid {
    display: grid;
    grid-template-columns:
      auto minmax(450px, max-content) minmax(450px, max-content)
      auto;
  }
  .section-two-introduction {
    display: flex;
    width: 444px;
    height: 139px;
    flex-direction: column;
    justify-content: center;
    flex-shrink: 0;
  }
  .introduction-part-one {
    color: #000;
    font-family: Source Sans Pro;
    font-size: 33px;
    font-style: normal;
    font-weight: 600;
    line-height: 36px; /* 109.091% */
  }
  .introduction-part-two {
    color: #9a8f8f;
    font-family: Source Sans Pro;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: 36px;
  }
  .skill-bubble {
    width: 350px;
    height: 60px;
    flex-shrink: 0;
    margin-top: 23px;
    margin-bottom: 23px;
    border-radius: 20px;
    background: linear-gradient(180deg, #32cdc3 0%, #3282c3 100%);
    display: flex;
  }
  .skill-image {
    width: 41.393px;
    height: 39px;
    flex-shrink: 0;
    border-radius: 384px;
    margin: auto;
  }
  .skill-name {
    display: flex;
    width: 86px;
    height: 19px;
    margin-top: 20px;
    margin-bottom: 21px;
    flex-direction: column;
    justify-content: center;
    flex-shrink: 0;
    color: #000;
    font-family: Source Sans Pro;
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: 36px; /* 180% */
  }
  .skill-description {
    display: flex;
    flex-direction: column;
    justify-content: center;
    flex-shrink: 0;
    color: #000;
    text-align: center;
    font-family: Source Sans Pro;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: 18px; /* 150% */
  }
  .section-two-picture {
    margin-top: 50px;
    width: 255px;
    height: 313px;
    flex-shrink: 0;
    border-radius: 59px;
    background: lightgray 50% / cover no-repeat;
  }
  .section-three {
    text-align: center;
    grid-row: 3;
  }
  .section-three-line {
    margin: auto;
    width: 53.19%;
    border-top: 1px solid black;
  }
  .section-three-experience {
    color: black;
    font-family: Source Sans Pro;
    font-size: 33px;
    font-style: normal;
    font-weight: 600;
    margin: auto;
    margin-top: 34px;
  }
  .section-three-subtitle {
    margin: auto;
    margin-bottom: 55px;
    color: black;
    font-family: Source Sans Pro;
    font-size: 18px;
    font-style: normal;
    font-weight: 300;
  }
  .section-four {
    grid-row: 4;
    align-items: center;
  }
  .tile-row {
    display: flex;
    justify-content: center;
  }
  .top-experience-tile {
    width: 260px;
    height: 196px;
    flex-shrink: 0;
    border-radius: 23px;
    background: linear-gradient(230deg, #000 13.47%, #3282c3 49.53%);
    box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25) inset;
    margin-right: 95px;
  }
  .bottom-experience-tile {
    width: 260px;
    height: 196px;
    flex-shrink: 0;
    border-radius: 23px;
    background: linear-gradient(230deg, #000 13.47%, #3282c3 49.53%);
    box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25) inset;
    margin-top: 51px;
    margin-left: 95px;
  }
  .section-five {
    display: flex;
    grid-row: 5;
    justify-content: center;
  }
  .lower-icons {
    border-radius: 30px;
    width: 400px;
    height: 77px;
  }
  .section-six {
    grid-row: 6;
  }
  .section-six-line {
    width: 100%;
    border-top: 1px solid black;
  }
  .working-with-me {
    display: flex;
    width: 694px;
    height: 35px;
    flex-direction: column;
    flex-shrink: 0;
    margin: auto;
    margin-top: 28px;
    color: black;
    font-family: Source Sans Pro;
    font-size: 33px;
    font-style: normal;
    font-weight: 600;
    line-height: 36px;
  }
  .contact-me {
    display: flex;
    width: 380px;
    height: 51px;
    margin: auto;
    margin-bottom: 2%;
    margin-top: 2%;
    flex-shrink: 0;
    position: relative;
    border-radius: 105px;
    background: linear-gradient(330deg, #32cdc3 47.67%, #3282c3 60.89%);
  }
  .contact-me-text {
    margin: 5px 0% 0% 20%;
    color: black;
    font-family: Source Sans Pro;
    font-size: 33px;
    font-weight: 600;
  }
  .section-six-send {
    width: 41.393px;
    height: 39px;
    flex-shrink: 0;
    border-radius: 384px;
    margin: auto;
  }
</style>
