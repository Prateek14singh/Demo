
 
  <script>
     import { onMount } from "svelte";
    import "../app.css";
 
  onMount(async () => {
    await import("tw-elements");
  });
</script>
  <slot />