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
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 3rem;
    letter-spacing: 0.05rem;
  }
  .normal {
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 0.025rem;
  }
</style>
