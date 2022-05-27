<script>
  import { logo } from '@assets';
</script>

<header class="h-20 | font-raleway">
  <div class="full-bounding h-full w-full mx-auto | flex items-center justify-between">
    <img class="h-6 lg:h-10" src={logo} alt="" height="24" />
    <nav class="text-sm md:text-base lg:text-lg">
      <ul class="flex items-center gap-6 md:gap-10 lg:gap-18">
        <li>
          <a
            class="transition hover:text-white focus:(text-white underline underline-white)"
            href="#features">
            Features
          </a>
        </li>
        <li>
          <a
            class="transition hover:text-white focus:(text-white underline underline-white)"
            href="/#team">
            Team
          </a>
        </li>
        <li>
          <a
            class="transition hover:text-white focus:(text-white underline underline-white)"
            href="/#sign_in">
            Sign In
          </a>
        </li>
      </ul>
    </nav>
  </div>
</header>
