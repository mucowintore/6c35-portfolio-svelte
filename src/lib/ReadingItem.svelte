<script>
  import { base } from '$app/paths';

  export let data = {};

  $: imageSrc = data.image && data.image.startsWith('http')
    ? data.image
    : `${base}${data.image ?? ''}`;
</script>

<article>
  <img src={imageSrc} alt="" />
  <h3>{data.title}</h3>
  <p>{data.author}</p>
</article>

<style>
  article {
    display: grid;
    gap: 0.5em;
    padding: 0.75em;
    border: 1px solid #ddd;
    border-radius: 0.5em;
  }

  h3,
  p {
    margin: 0;
  }

  img {
    max-width: 100%;
    height: auto;
  }
</style>
