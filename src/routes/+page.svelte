<script>
  import { base } from '$app/paths';
  import projects from '$lib/projects.json';
  import reading from '$lib/reading.json';
  import Project from '$lib/Project.svelte';
  import ReadingItem from '$lib/ReadingItem.svelte';
</script>

<svelte:head>
  <title>Muco: Personal site and portfolio</title>
</svelte:head>

<main>
  <h1>Muco</h1>
  <nav aria-label="Primary">
    <a class="current" href=".">Home</a>
    <a href="projects">Projects</a>
    <a href="contact">Contact</a>
    <a href="resume">Resume</a>
    <a href="https://github.com/mucowintore" target="_blank" rel="noopener noreferrer">GitHub</a>
  </nav>
  <p>I am Muco and this is my portfolio website. Stay tuned for awesome content coming up!</p>
  <img src="{base}/images/profile.jpg" alt="Portrait of Muco" />

  <h2>Latest Projects</h2>
  <div class="projects highlights">
    {#each projects.slice(0, 3) as p}
      <Project data={p} />
    {/each}
  </div>

  <h2>What I’m Reading</h2>
  <div class="projects reading-list">
    {#each reading as item}
      <ReadingItem data={item} />
    {/each}
  </div>
</main>
