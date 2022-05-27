<script>
  export let layout = '';
</script>

<section
  class="max-w-xs w-full mx-auto p-8 | space-y-9 | bg-dark-800 rounded-lg {layout} | sm:max-w-md md:max-w-xl lg:max-w-3xl">
  <div class="flex flex-col gap-4 | text-center">
    <h2 class="text-lg md:text-xl">Get early access today</h2>
    <p>
      It only takes a minute to sign up and our free starter tier is extremely generous. If you have
      any questions, our support team would be happy to help you.
    </p>
  </div>
  <form class="flex flex-col gap-6 | lg:flex-row">
    <div class="w-full">
      <label class="sr-only" for="email">Email</label>
      <input
        class="w-full h-12 px-6 | bg-white rounded-full text-blue-900
        focus:(ring-2 ring-cyan)"
        type="text"
        name="email"
        id="email"
        placeholder="email@example.com" />
    </div>
    <button class="button button--cyan w-full px-12 | lg:max-w-[fit-content]">
      Get Started For Free
    </button>
  </form>
</section>
