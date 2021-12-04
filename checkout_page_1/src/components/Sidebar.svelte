<script>
  import PaymentMethod from "./PaymentMethod.svelte"
  import PaymentCreditCard from "./PaymentCreditCard.svelte"
  import Button from "./Button.svelte"
  import Typography from "./Typography.svelte"
  import Divider from "./Divider.svelte"
  let paymentMethod = ["Online Payment", "Cash On Delivery"]
</script>

<div class="p-5">
  <Typography text="Payment" type="title" color="#f7f7f7" />
  <Divider color="#f7f7f7" />
  <PaymentMethod methods={paymentMethod} />
  <PaymentCreditCard />
  <Button text="CHECKOUT" />
</div>
