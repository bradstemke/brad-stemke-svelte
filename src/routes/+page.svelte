<script>
  import Footer from "$lib/Footer.svelte";
</script>

<h1>Brad Stemke</h1>

<Footer />

<style>
  :root {
    /* Colors */
    --color-primary-yellow: rgb(243, 175, 89);
    --color-primary-tan: rgb(248, 247, 243);
    --color-primary-red: rgb(189, 75, 47);
    --color-primary-blue: rgb(30, 74, 159);
    --color-primary-green: rgb(38, 77, 68);
    --color-primary-white: rgb(248, 245, 241);

    /* Spacing  */
    --spacing-1: 0.5rem;
    --spacing-2: 1rem;
    --spacing-3: 1.5rem;
    --spacing-4: 2rem;
    --spacing-5: 2.5rem;
    --spacing-6: 3rem;
    --spacing-7: 3.5rem;
    --spacing-8: 4rem;

    /* Typography */
    font-family: 'Space Mono', monospace;
    font-size: 16px;
    font-variant-ligatures: none;
    line-height: 1.4;  
  }
  
  /* List Resets  */
  :global(ul, ol) {
    margin: 0;
    padding: 0;
  } 
</style>