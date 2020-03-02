<script>
// export let expense
// let {name, amount} = expense
// Another method below
export let id;
export let name = "";
export let amount =0;
let displayAmount = false;
function toggleAmount = () {
    displayAmount = !displayAmount
}
</script>

<article class="single-expense">
    <div class="expense-infor">
        <h2>{name} 
            <button class="amount-btn" on:click={toggleAmount}>
                <i class="fas fa-caret-down" />
            </button>
        </h2>
        {#if displayAmount}
        <h4>amount: ${amount}</h4>
        {/if}
    </div>
    <div class="expense-button">
        <button class="expense-btn edit-btn">
            <i class="fas fa-pen" />
        </button>
          <button class="expense-btn delete-btn">
            <i class="fas fa-trash" />
        </button>
    </div>
</article>
