<script>
  import "../app.css";
  import Navbar from "components/navbar.svelte";

</script>

<div class="p-4">
  <Navbar />
  <main class="max-w-8xl mx-auto xl:mx-64 sm:mx-32 p-4 sm:p-6 md:p-8">
    <slot />
  </main>
</div>