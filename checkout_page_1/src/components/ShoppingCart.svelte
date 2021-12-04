<script>
  import ShoppingCartItem from "./ShoppingCartItem.svelte"
  import Typography from "./Typography.svelte"
  import Divider from "./Divider.svelte"
  import { prevent_default } from "svelte/internal"
  export let items = [
    {
      title: "Pancake",
      desc: "Sweetest pancake ever made !",
      pict: "img/cera-SxTlB4fde9Q-unsplash.jpg",
      qty: 1,
      price: 15000
    },
    {
      title: "Sweet bread",
      desc: "Best dish for your breakfast, it is so yummy and many people love it.",
      pict: "img/joseph-gonzalez-zcUgjyqEwe8-unsplash.jpg",
      qty: 2,
      price: 17000
    }
  ]
  let formatter = new Intl.NumberFormat("id-ID", {
    style: "currency",
    currency: "IDR"
  })
  let subtotal = items.reduce((prev, curr) => {
    return prev + curr.qty * curr.price
  }, 0)
</script>

<div class="p-3">
  <Typography text="Shopping Cart" type="title" />
  <div class="shopping-cart">
    {#each items as item}
      <ShoppingCartItem {...item} />
    {/each}
  </div>
  <Divider color="#aaa" />
  <div class="shopping-cart-summary">
    <Typography text="Subtotal" type="subtitle" />
    <Typography text={formatter.format(subtotal)} type="subtitle" />
  </div>
</div>

<style>
  .shopping-cart-summary {
    display: flex;
    justify-content: space-between;
  }
</style>
