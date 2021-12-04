<script>
  import Typography from "./Typography.svelte"
  export let methods = []
</script>

<div class="payment-method">
  {#each methods as m}
    <div class="payment-method-item">
      <label for="payment-method-item-cod">
        <Typography text={m} color="#f7f7f7" />
        <input type="radio" name="payment_method" />
        <span class="checkmark" />
      </label>
    </div>
  {/each}
</div>

<style>
  .payment-method {
    padding-top: 1rem;
    padding-bottom: 1rem;
  }
  .payment-method-item {
    display: block;
    position: relative;
    padding-left: 2rem;
    margin-bottom: 1rem;
    cursor: pointer;
    font-size: 12px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
  }

  .payment-method-item input {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    margin: 0;
    z-index: 2;
    opacity: 0;
    cursor: pointer;
  }

  .checkmark {
    position: absolute;
    top: 0;
    left: 0;
    height: 18px;
    width: 18px;
    border-radius: 50%;
    border-color: #f7f7f7;
    border-style: solid;
    border-width: 2px;
  }

  /* On mouse-over, add a grey background color */
  .payment-method-item:hover input ~ .checkmark {
    background-color: #f7f7f735;
  }

  /* Create the indicator (the dot/circle - hidden when not checked) */
  .checkmark:after {
    content: "";
    position: absolute;
    display: none;
  }

  /* Show the indicator (dot/circle) when checked */
  .payment-method-item input:checked ~ .checkmark:after {
    display: block;
  }

  /* Style the indicator (dot/circle) */
  .payment-method-item .checkmark:after {
    top: 4px;
    left: 4px;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: white;
  }
</style>
