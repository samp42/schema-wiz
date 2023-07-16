<!--
<dialog bind:this={dialog} on:close>
    <slot/>
</dialog> -->
<script>
    export let newInstanceDialog
</script>

<dialog id="my_modal_3" class="modal" bind:this={newInstanceDialog}>
    <form method="dialog" class="modal-box">
      <button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
      <h3 class="font-bold text-lg">Hello!</h3>
      <p class="py-4">Press ESC key or click on ✕ button to close</p>
    </form>
</dialog>