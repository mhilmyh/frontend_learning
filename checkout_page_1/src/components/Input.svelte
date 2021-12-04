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
  label {
    display: block;
  }
  input {
    font-size: 16px;
    font-size: max(16px, 1em);
    font-family: inherit;
    padding: 0.25em 0.5em;
    background-color: rgba(255, 255, 255, 0);
    color: #f7f7f7;
    border: 2px solid #f7f7f7aa;
    border-left: 0;
    border-right: 0;
    border-top: 0;
    line-height: 1;
    height: 2.25rem;
    width: 100%;
    display: block;
  }
  input:focus {
    background-color: rgba(255, 255, 255, 0.1);
    border-top-left-radius: 4px;
    border-top-right-radius: 4px;
    transition: 180ms box-shadow ease-in-out;
    outline: 1px solid transparent;
  }
</style>
