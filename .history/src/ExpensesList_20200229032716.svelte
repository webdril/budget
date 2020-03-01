<script>
import SectionTitle from './Title.svelte';
imprt expense from '.expense.svelte';
export let expenses = [];
</script>

<section>
    <SectionTitle title= 'expense list' />
    <ul>
    {#each expenses as expense}

    {/each}
    </ul>
</section>