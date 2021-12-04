<div id="checkout-button">
  <button>
    <slot />
  </button>
</div>

<style>
  button {
    border-radius: 8px;
    border-width: 0;
    padding-left: 0.5rem;
    padding-right: 0.5rem;
    padding-top: 0.25rem;
    padding-bottom: 0.25rem;
    background-color: #ebc934;
    font-weight: 700;
    letter-spacing: 0.05rem;
    float: right;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;
  }
  button:hover {
    box-shadow: rgba(125, 125, 125, 0.1) 0px 20px 25px -5px,
      rgba(255, 255, 255, 0.1) 0px 10px 10px -5px;
  }
  button:active {
    background-color: #d1b01d;
  }
</style>
