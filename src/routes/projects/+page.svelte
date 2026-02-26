<script>
  import projects from '$lib/projects.json';
  import Project from '$lib/Project.svelte';
</script>

<svelte:head>
  <title>Projects</title>
</svelte:head>

<main>
  <h1>{projects.length} Projects</h1>
  <nav aria-label="Primary">
    <a href=".">Home</a>
    <a class="current" href="projects">Projects</a>
    <a href="contact">Contact</a>
    <a href="resume">Resume</a>
    <a href="https://github.com/mucowintore" target="_blank" rel="noopener noreferrer">GitHub</a>
  </nav>
  <div class="projects">
    {#each projects as p}
      <Project data={p} />
    {/each}
  </div>
</main>
