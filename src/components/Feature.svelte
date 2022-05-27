<script lang="ts">
  export let title: string;
  export let icon: string;
</script>

<article class="flex flex-col items-center gap-9">
  <img src={icon} alt="" />
  <div class="flex flex-col gap-3 text-center">
    <h3 class="text-xl | md:text-2xl">{title}</h3>
    <p class="text-sm | md:text-base">
      <slot />
    </p>
  </div>
</article>
