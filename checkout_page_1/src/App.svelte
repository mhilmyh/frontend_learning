<script>
  import ShoppingCart from "./components/ShoppingCart.svelte"
  import Sidebar from "./components/Sidebar.svelte"
</script>

<main class="container">
  <div class="side-left">
    <ShoppingCart />
  </div>
  <div class="side-right">
    <Sidebar />
  </div>
</main>

<style>
  .side-left {
    background-color: #f7f7f7;
    width: 65%;
  }
  .side-right {
    background-color: #343434;
    width: 35%;
  }
  .container {
    display: flex;
    min-height: 100vh;
  }
</style>
