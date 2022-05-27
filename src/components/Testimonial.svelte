<script lang="ts">
  export let name: string;
  export let title = 'Founder & CEO, Huddle';
  export let image: string;
</script>

<article class="p-6 | space-y-6 | bg-dark-700 rounded-md">
  <blockquote>
    <p class="text-xs | md:text-sm">
      <slot />
    </p>
  </blockquote>
  <header class="flex items-center gap-3">
    <img class="h-10 w-10 min-w-10 | rounded-full" src={image} alt={name} />
    <div class="flex flex-col gap-1">
      <h3 class="text-sm ">{name}</h3>
      <span class="text-xs"> {title}</span>
    </div>
  </header>
</article>
