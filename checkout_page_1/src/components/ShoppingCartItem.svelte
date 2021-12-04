<script>
  import Typography from "./Typography.svelte"

  export let title = ""
  export let desc = ""
  export let pict = ""
  export let qty = 0
  export let price = 0

  let formatter = new Intl.NumberFormat("id-ID", {
    style: "currency",
    currency: "IDR"
  })
</script>

<div class="shopping-cart-item">
  <div class="product-image">
    <img src={pict} alt="product-preview" />
  </div>
  <div class="product">
    <div class="product-title">
      <Typography text={title} type="title" />
    </div>
    <div class="product-subtitle">
      <Typography text={desc} type="normal" />
    </div>
  </div>
  <div class="product-button-quantity">{qty} pcs</div>
  <div class="product-button-price">{formatter.format(price)}</div>
</div>

<style>
  .shopping-cart-item {
    display: grid;
    grid-template-columns: 20% 50% 15% 15%;
    justify-content: space-around;
    align-items: center;
    padding: 0.5rem;
  }
  .shopping-cart-item .product {
    display: block;
  }
  .product-image {
    display: block;
  }
  .product-image img {
    border-radius: 8px;
    max-width: 128px;
    object-fit: contain;
  }
</style>
