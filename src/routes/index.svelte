<script>
  import Title from "../lib/title.svelte";
  import Index from "./index.svelte";
  let title = "Ninja Gaming Guides";
  const updateTitle = () => {
    title = "something completely different";
  };
</script>

<div class="index">
  <!-- <h1>{title}</h1> -->
  <p>
    Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
  </p>

  <button on:click={updateTitle}>change title</button>
  <input type="text" bind:value={title} />

  <a href="/about">about</a>
  <a href="/guides">guides</a>
</div>

<style>
  .index {
    text-align: center;
    display: block;
    margin: 20px auto;
  }
</style>
