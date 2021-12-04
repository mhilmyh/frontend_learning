<script>
  import Typography from "./Typography.svelte"
  export let value = ""
  export let name = ""
  export let type = ""
  export let label = ""
</script>

<div class="container">
  <label for="input-{type}-{name}">
    <Typography text={label} color="#f7f7f7" />
  </label>
  <input id="input-{type}-{name}" class="input" {value} {type} />
</div>

<style>
  .container {
    margin: 0;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  input {
    font-size: 16px;
    font-size: max(16px, 1em);
    font-family: inherit;
    padding: 0.25em 0.5em;
    background-color: #fff;
    border: 2px solid #8b8a8b;
    border-radius: 4px;
  }

  input {
    line-height: 1;
    height: 2.25rem;
  }
  input:focus {
    border-color: hsl(245, 100%, 42%);
    box-shadow: 0 0 0 3px hsla(245, 100%, calc(42% + 40%), 0.8);
    transition: 180ms box-shadow ease-in-out;
    outline: 3px solid transparent;
  }
</style>
