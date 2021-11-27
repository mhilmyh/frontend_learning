<script>
  export let type = "normal"
  export let color = "#000"
  export let text = ""
</script>

<span class={type} style="color: {color};">
  {text}
</span>

<style>
  .title {
    font-size: larger;
    font-weight: bolder;
  }
  .normal {
    font-size: medium;
    font-weight: normal;
  }
</style>
