<script>
  import { logo } from '@assets';
</script>

<footer class="pb-12 | bg-blue-900 | md:pb-18 lg:pb-24">
  <!-- * Container -->
  <div class="full-bounding mx-auto | flex flex-col gap-12">
    <div class="flex flex-col gap-9">
      <div>
        <img src={logo} alt="Fylo" />
      </div>
      <div class="flex flex-col gap-9 lg:flex-row">
        <address class="flex flex-col gap-3 lg:(flex-row gap-12)">
          <div class="lg:max-w-xs | flex gap-4">
            <i class="bx bxs-map mt-1 text-2xl" />
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua
            </p>
          </div>

          <div class="flex flex-col gap-3">
            <div class="flex gap-4 items-center">
              <i class="bx bxs-phone-call mt-1 text-2xl" />
              <span> +1-543-123-4567 </span>
            </div>
            <div class="flex gap-4 items-center">
              <i class="bx bxl-gmail mt-1 text-2xl" />
              <span> example@fylo.com </span>
            </div>
          </div>
        </address>
        <!--* Navigation -->
        <nav class="flex flex-col gap-9 lg:(flex-row ml-auto mr-3) xl:(gap-18 mr-12)">
          <ul class="space-y-4">
            <li>
              <a class="link" href="#69"> About Us </a>
            </li>
            <li>
              <a class="link" href="#69"> Jobs </a>
            </li>
            <li>
              <a class="link" href="#69"> Press </a>
            </li>
            <li>
              <a class="link" href="#69"> Blog </a>
            </li>
          </ul>
          <ul class="space-y-4">
            <li>
              <a class="link" href="#69"> Contact Us</a>
            </li>
            <li>
              <a class="link" href="#69"> Terms </a>
            </li>
            <li>
              <a class="link" href="#69"> Privacy </a>
            </li>
          </ul>
        </nav>
        <!-- * Social Media -->
        <div
          class="flex items-center justify-center gap-3 | lg:items-start @lg:(flex-col justify-start)">
          <button class="button--social h-8 w-8 min-w-8 | border-1.5px border-white rounded-full">
            <span class="sr-only">Follow us on Facebook</span>
            <i class="bx bxl-facebook" />
          </button>
          <button class="button--social h-8 w-8 min-w-8 | border-1.5px border-white rounded-full">
            <span class="sr-only">Follow us on Twitter</span>
            <i class="bx bxl-twitter" />
          </button>
          <button class="button--social h-8 w-8 min-w-8 | border-1.5px border-white rounded-full">
            <span class="sr-only">Follow us on Instagram</span>
            <i class="bx bxl-instagram" />
          </button>
        </div>
      </div>
    </div>
  </div>
</footer>

<style>
  .link {
    @apply transition hover:text-white focus:(text-white font-bold);
  }

  .button--social {
    @apply transition hover:(text-cyan border-cyan) focus:(text-cyan border-cyan);
  }
</style>
