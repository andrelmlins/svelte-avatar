<script>
  import { Highlight } from 'svelte-highlight';
  import { javascript } from 'svelte-highlight/languages';

  import Avatar from '../../src/Avatar.svelte';

  $: code = `<Avatar square name="John Walker" />`;
</script>

<style>
  div {
    padding: 1rem 0;
  }
</style>

<div>
  <h2>Square</h2>
  <Avatar square name="John Walker" />
  <Highlight language={javascript} {code} />
</div>
