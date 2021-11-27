<script>
</script>

<!-- Container -->
<main class="shopping-cart">
  <h1>Shopping Cart</h1>
  <div class="cart">
    <div class="cart-item">
      <div class="product-image">
        <img src="" alt="product-preview" />
      </div>
      <div class="product-name">
        <h3>grilled chicken mushroom</h3>
        <p>Served with 2 side dishes rice. French fries, mashed potato, vegetables.</p>
      </div>
      <div class="product-button-price" />
      <div class="product-button-quantity" />
      <div class="product-button-remove">
        <button>X</button>
      </div>
    </div>
  </div>
  <div id="cart-summary" />
</main>

<div id="sidebar">
  <h1>Payment</h1>
  <div class="payment-method">
    <div class="payment-method-item">
      <input type="radio" id="payment-method-item-cod" name="payment-method-item" value="" />
      <label for="payment-method-item-cod">COD (Cash On Delivery)</label>
    </div>
    <div class="payment-method-item">
      <input type="radio" id="payment-method-item-online" name="payment-method-item" value="" />
      <label for="payment-method-item-online">Online Payment</label>
    </div>
  </div>

  <div id="credit-card">
    <div id="credit-card-name">
      <input type="text" name="credit-card-name" value="" />
    </div>
    <div id="credit-card-number">
      <input type="text" name="credit-card-number" value="" />
    </div>
    <div id="credit-card-exp-date">
      <input type="text" name="credit-card-exp-date" value="" />
    </div>
    <div id="credit-card-cvv">
      <input type="text" name="credit-card-cvv" value="" />
    </div>
  </div>

  <div id="checkout-button">
    <button>checkout</button>
  </div>
</div>
