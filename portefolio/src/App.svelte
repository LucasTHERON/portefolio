<script>
  import Accueil from "./lib/Accueil.svelte";
  import Competences from "./lib/Competences.svelte";
  import Projets from "./lib/Projets.svelte";
  let content = 'accueil';
</script>

<main>
<div class="main-container {content}">


  <nav>
    <button on:click={() => content = 'accueil'}>Accueil</button>
    <button on:click={() => content = 'competences'}>Compétences</button>
    <button on:click={() => content = 'projets'}>Projets</button>
  </nav>
  
  <div><h1>
    {#if content == 'accueil'}
    <Accueil />
    {:else if content == 'competences'}
    <Competences />
    {:else if content == 'projets'}
    <Projets />
    {:else}
    <h1>404</h1>
    {/if}        
  </h1></div>

</div>


</main>

<style>
</style>
