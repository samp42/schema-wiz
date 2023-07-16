<script lang="ts">
  import NewInstanceDialog from "./components/NewInstanceDialog.svelte";
  let newInstanceDialog;
</script>

<main class="container">
  <h1>Welcome to Schema Whiz! 🧙‍♂️🪄</h1>

  <div>
    <p>To start, add a database instance</p>
    <button class="btn btn-primary" on:click={() => {newInstanceDialog.showModal()}}>Add database</button>
  </div>

  <NewInstanceDialog bind:newInstanceDialog on:close={() => console.log('closed')}>
    This is amazingly simple! (press esc to close)
  </NewInstanceDialog>
</main>

<style>
</style>