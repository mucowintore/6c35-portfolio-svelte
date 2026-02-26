<svelte:head>
  <title>Contact</title>
</svelte:head>

<main>
  <h1>Contact</h1>
  <nav aria-label="Primary">
    <a href=".">Home</a>
    <a href="projects">Projects</a>
    <a class="current" href="contact">Contact</a>
    <a href="resume">Resume</a>
    <a href="https://github.com/mucowintore" target="_blank" rel="noopener noreferrer">GitHub</a>
  </nav>
  <p>This form opens your email client with a draft message so you can reach out quickly.</p>
  <form action="mailto:16810076+mucowintore@users.noreply.github.com" method="GET">
    <label>
      <span>Email</span>
      <input type="email" name="email" value="test@example.com" required />
    </label>
    <label>
      <span>Subject</span>
      <input name="subject" value="Hello from your site" />
    </label>
    <label>
      <span>Message</span>
      <textarea name="body" rows="3">This is a test message.</textarea>
    </label>
    <button type="submit">Send</button>
  </form>
</main>
