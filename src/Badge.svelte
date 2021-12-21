<script>
  import { Image } from "sveltestrap";
  export let certName;
  export let name;
  export let url = false;

  let src = "/img/" + name;
  let certIdClassName = "text-secondary";
  let certIcom = "";
  if (url) {
    src += "-passed";
    certIdClassName = "fw-bold";
    certIcom = "&nbsp;✅"
  }
  src += ".png";
</script>

{#if url && url != "#"}
  <a href={url} target="_blank"><Image {src} /></a>
{:else}
  <Image {src} />
{/if}
<div class={certIdClassName}>{certName}{@html certIcom}</div>