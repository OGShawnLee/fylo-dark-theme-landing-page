<script lang="ts" context="module">
  function isEmpty(str: string) {
    return str.trim().length === 0;
  }

  function isValidEmail(email: string | null) {
    if (!email || isEmpty(email)) return false;
    const validRegex = /^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/;
    return validRegex.test(email);
  }
</script>

<script lang="ts">
  export let layout = '';
  export let state: 'IDLE' | 'ERROR' | 'SUCCESS' = 'IDLE';

  let email: string;

  $: if (email && (state === 'ERROR' || state === 'SUCCESS')) state = 'IDLE';
  $: isError = state === 'ERROR';

  function handleSubmit() {
    state = isValidEmail(email) ? 'SUCCESS' : 'ERROR';
    email = '';
  }
</script>

<section
  class="max-w-xs w-full mx-auto py-12 px-8 | space-y-9 | bg-dark-800 rounded-lg {layout} | sm:max-w-md md:max-w-xl lg:max-w-3xl">
  <div class="flex flex-col gap-4 | text-center">
    <h2 class="text-lg md:text-xl">Get early access today</h2>
    <p>
      It only takes a minute to sign up and our free starter tier is extremely generous. If you have
      any questions, our support team would be happy to help you.
    </p>
  </div>
  <form class="relative flex flex-col gap-6 | lg:flex-row" on:submit|preventDefault={handleSubmit}>
    <div class="relative | w-full">
      <label class="sr-only" for="email">Email</label>
      <input
        class="w-full h-12 px-6 | bg-white rounded-full text-blue-900
        focus:ring-2 | <md:text-sm {isError ? 'focus:ring-red' : 'focus:ring-cyan'}"
        name="email"
        id="email"
        placeholder="email@example.com"
        bind:value={email} />
    </div>
    <button class="button button--cyan w-full px-12 | lg:max-w-[fit-content]">
      Get Started For Free
    </button>
    {#if state === 'ERROR' || state === 'SUCCESS'}
      <div
        class="min-w-[fit-content] absolute -bottom-6.5 | transform lg:left-3 <lg:(right-1/2 translate-x-1/2)">
        <span class="text-xs {isError ? 'text-red' : 'text-cyan'} font-bold">
          {isError ? 'Please enter a valid email address' : 'Thank You!'}
        </span>
      </div>
    {/if}
  </form>
</section>
