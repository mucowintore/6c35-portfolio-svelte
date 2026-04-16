<script>
  export let data = {};
</script>

<article>
  <h2>{data.title}</h2>
  <p class="year">{data.year}</p>
  <p class="description">{data.description}</p>
  {#if data.url}
    <p class="link-row">
      <a href={data.url} target="_blank" rel="noreferrer">Explore project</a>
    </p>
  {/if}
  <img src={data.image} alt="" />
</article>

<style>
  article {
    display: flex;
    flex-direction: column;
    gap: 0.45em;
    padding: 0.75em;
    border: 1px solid #ddd;
    border-radius: 0.5em;
  }

  h2 {
    margin: 0;
  }

  .year {
    margin: 0;
    font-size: 0.9rem;
    font-weight: 600;
    color: color-mix(in oklch, currentColor, canvas 35%);
  }

  .description {
    margin: 0;
  }

  img {
    margin-top: 0.2rem;
    max-width: 100%;
    height: auto;
  }

  .link-row {
    margin: 0.2rem 0 0;
  }

  a {
    font-weight: 600;
  }
</style>
