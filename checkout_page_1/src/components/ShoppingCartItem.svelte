<script>
  import Typography from "./Typography.svelte"

  export let title = ""
  export let desc = ""
</script>

<div class="shopping-cart-item">
  <div class="product-image">
    <img src="" alt="product-preview" />
  </div>
  <div class="product-name">
    <Typography text={title} type="title" />
    <Typography text={desc} type="normal" />
  </div>
  <div class="product-button-price" />
  <div class="product-button-quantity" />
  <div class="product-button-remove">
    <button>X</button>
  </div>
</div>
