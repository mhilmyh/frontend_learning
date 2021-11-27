<script>
  export let type = "normal"
  export let color = "#000"
</script>

<span class={type} style="color: {color};">
  <slot />
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
