<script>
  export let pokeman;
  import { fade } from 'svelte/transition'
</script>

<a
  transition:fade
  class="p-6 bg-gray-100 text-gray-800 text-center rounded-md shadow-sm hover:shadow-md flex flex-col items-center"
  href={`/pokemon/${pokeman.id}`}>
  <img class="h-30" src="{pokeman.image}" alt={pokeman.name} />
  <h2>{pokeman.id}. {pokeman.name}</h2>
</a>
