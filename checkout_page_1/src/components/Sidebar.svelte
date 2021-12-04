<script>
  import PaymentMethod from "./PaymentMethod.svelte"
  import PaymentCreditCard from "./PaymentCreditCard.svelte"
  import Button from "./Button.svelte"
  import Typography from "./Typography.svelte"
  let paymentMethod = ["Online Payment", "Cash On Delivery"]
</script>

<div class="p-3">
  <Typography text="Payment" type="title" color="#f7f7f7" />
  <PaymentMethod methods={paymentMethod} />
  <PaymentCreditCard />
  <Button>
    <span>Checkout</span>
    <svg
      xmlns="http://www.w3.org/2000/svg"
      class="icon-arrow-right"
      width="24"
      height="24"
      viewBox="0 0 24 24"
      stroke-width="2"
      stroke="currentColor"
      fill="none"
      stroke-linecap="round"
      stroke-linejoin="round"
    >
      <path stroke="none" d="M0 0h24v24H0z" fill="none" />
      <line x1="5" y1="12" x2="19" y2="12" />
      <line x1="13" y1="18" x2="19" y2="12" />
      <line x1="13" y1="6" x2="19" y2="12" />
    </svg>
  </Button>
</div>

<style>
  .icon-arrow-right {
    padding: 0.25rem;
  }
</style>
