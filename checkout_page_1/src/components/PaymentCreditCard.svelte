<script>
  import Input from "./Input.svelte"
</script>

<form autocomplete="off" class="credit-card">
  <Input type="text" name="credit-card-name" label="Cardholder Name" />
  <Input type="text" name="credit-card-number" label="Card Number" />
  <Input type="text" name="credit-card-exp-date" label="Expire Date" />
  <Input type="text" name="credit-card-cvv" label="CVV" />
</form>

<style>
  .credit-card {
    padding-bottom: 1rem;
  }
</style>
