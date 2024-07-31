<script>
  import Product from "./product.svelte";

  let new_fruit = [
    { name: "Apple", price: 160 },
    { name: "Orange", price: 80 },
    { name: "mango", price: 100 },
  ];
</script>

{#each new_fruit as fruits}
  <Product fruit={fruits.name} price={fruits.price} />
{/each}
