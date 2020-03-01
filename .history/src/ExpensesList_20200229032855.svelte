<script>
import SectionTitle from './Title.svelte';
import expense from './Expense.svelte';
export let expenses = [];
</script>

<section>
    <SectionTitle title= 'expense list' />
    <ul>
        {#each expenses as expense}
    ``````<Expense />
        {/each}
    </ul>
</section>