<script>
  import Header from './component/Header.svelte';
  import Hero from './component/Hero.svelte';
  import Services from './component/Services.svelte';
  import Portfolio from './component/Portfolio.svelte';
  import Testimonials from './component/Testimonials.svelte';
  import Cta from './component/Cta.svelte';
  import Team from './component/Team.svelte';
  import Contact from './component/Contact.svelte';
  import Footer from './component/Footer.svelte';
  import About from './component/About.svelte';
  import FeatureService from './component/FeatureService.svelte';
  import Count from './component/Count.svelte';
</script>

<link rel="stylesheet" href="styles.css" />

<main>
  <Header />
  <Hero />
  <FeatureService />
  <About />
  <Services />
  <Count />
  <Portfolio />
  <Testimonials />
  <Cta />
  <Team />
  <Contact />
</main>

<Footer />
