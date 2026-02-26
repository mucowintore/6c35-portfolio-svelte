<script>
  import { base } from '$app/paths';
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
</main>
