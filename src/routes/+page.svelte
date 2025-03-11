<script>
    import Header from "../lib/components/header/navBar.svelte";
    import Footer from "../lib/components/footer/foot.svelte"; //contact
    import Home from "../lib/components/home/home.svelte";
    import About from "../lib/components/about/about.svelte";
    import Team from "../lib/components/team/team.svelte";
</script>

<Header /> <!--Nav bar-->
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
</style>
