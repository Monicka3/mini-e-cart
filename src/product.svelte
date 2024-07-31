<script>
  export let fruit;
  export let price
  let quantity = 0;

  function add() {
    quantity = quantity + 1;
  }
  function minus() {
    if(quantity>1)
    quantity = quantity - 1;
    else
    quantity=0
  }
</script>
{fruit}=${price}
<div>
  <button on:click={add}> +(add) </button>
  {quantity}
  <button on:click={minus}> -(minus) </button>
</div>
