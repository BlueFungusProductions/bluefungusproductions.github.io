<script>
    import Header from "../lib/components/header/navBar.svelte";
    import Footer from "../lib/components/footer/foot.svelte"; //contact
    import Home from "../lib/components/home/home.svelte";
    import About from "../lib/components/about/about.svelte";
    import Team from "../lib/components/team/team.svelte";
</script>

<Header /> <!--Nav bar-->
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
    .container {
        width: 100%;
        max-width: 1000px;
        margin: 0 auto;
    }
    
    .black {
    background: linear-gradient(to right, #0c0c0c 0%, #0c0c0c calc(50% - 700px), 
                                transparent calc(50% - 700px), transparent calc(50% + 700px), 
                                #0c0c0c calc(50% + 700px), #0c0c0c 100%);
    width: 100%;
    height: 1090px;
    position: absolute;
    top: 0;
    left: 0; 
    filter: blur(7px); 
}
</style>
