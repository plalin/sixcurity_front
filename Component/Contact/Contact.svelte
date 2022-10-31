<!--./src/Component/Contact/Contact.svelte-->
<script>
    //params라는 props를 받아온다.
    export let params;
  </script>
  <!-- if는 이후에 포스팅하겠다. -->
  {#if params}
    <h1>{params.test}</h1>
  {/if}
  <h1>Contact</h1>