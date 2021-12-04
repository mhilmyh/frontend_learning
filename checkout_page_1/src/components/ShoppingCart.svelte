<script>
  import ShoppingCartItem from "./ShoppingCartItem.svelte"
  import Typography from "./Typography.svelte"

  export let items = []
</script>

<div class="p-5">
  <Typography text="Shopping Cart" type="title" />
  <div class="shopping-cart">
    {#each items as item}
      <ShoppingCartItem title={item.title} desc={item.desc} />
    {/each}
  </div>
  <div class="shopping-cart-summary" />
</div>
