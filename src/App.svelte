<script>
  import './styles/app.css';
  import { Banner, Footer, Features, Header, Hero, Invitation, Testimonials } from '@layout';
</script>

<Header />

<main class="bg-dark-900 pb-80 | lg:pb-70">
  <h1 class="sr-only">Fylo</h1>
  <div class="full-bounding mx-auto | flex flex-col gap-32">
    <Hero />
    <Features />
    <Banner />
    <Testimonials />
  </div>
</main>

<div class="relative pt-68 | bg-blue-900 lg:pt-48">
  <Invitation layout="absolute bottom-full right-1/2 | transform translate-y-1/2 translate-x-1/2" />
  <Footer />
</div>
