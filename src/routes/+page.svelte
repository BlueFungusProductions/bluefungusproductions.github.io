<script>
  import Header from "../lib/components/header/navBar.svelte";
  import Footer from "../lib/components/footer/foot.svelte";
  import Home from "../lib/components/home/home.svelte";
  import About from "../lib/components/about/about.svelte";
  import Team from "../lib/components/team/team.svelte";
</script>

<Header />
<div class="black"></div>
<div class="container">
  <Home />

  <section id="about">
    <About />
  </section>

  <section id="team">
    <Team />
  </section>
</div>
<Footer />

<style>
  @font-face {
    font-family: FuzzyBubbles;
    src: url(../fonts/FuzzyBubbles.ttf);
  }

  @font-face {
    font-family: OldEnglishTextMT;
    src: url(../fonts/OldEnglishTextMT.ttf);
  }

  @font-face {
    font-family: OldNewspaperTypes;
    src: url(../fonts/OldNewspaperTypes.ttf);
  }
  .container {
    width: 100%;
    max-width: 1000px;
    margin: 0 auto;
  }

  .black {
    position: absolute;
    width: 100%;
    height: 1090px;
    top: 0;
    left: 0;
    background: linear-gradient(
      to right,
      #0c0c0c 0%,
      #0c0c0c calc(50% - 700px),
      transparent calc(50% - 700px),
      transparent calc(50% + 700px),
      #0c0c0c calc(50% + 700px),
      #0c0c0c 100%
    );
    filter: blur(7px);
  }
</style>
