<script>
import Title from './Title.svelte'
let name = "";
let amount = null;
export let addExpense;
// $: console.log({name, amount}); for checking reactivity

$: isEmpty = !name || !amount

function handleSubmit(){
    addExpense({name, amount})
}
</script>

<section class="form">

    <Title title= "add expense" />
    <form class="expense-form" on:submit|preventDefault={handleSubmit}>
        <div class="form-control">
            <label for="name">Name</label>
            <input type="text" id="name" bind:value={name} />
        </div>
        <div class="form-control">
            <label for="amount">amount</label>
            <input type="number" id="amount" bind:value={amount}/>
        </div>
        {#if isEmpty}
                <p class="form-empty">Please fill out all form field</p>

        {/if}
        <button type="submit" class="btn btn-block" class:disabled={isEmpty} disabled={isEmpty}>add expense</button >
        <button type="button" class="close-btn">
        <i class="fas fa-times" />close
        </button>
    </form>
</section>