<script>
    import SectionTitle from './Title.svelte';
    import Expense from './Expense.svelte';
import App from './App.svelte';
    export let expenses =[];
</script>

<section>
    <SectionTitle title="expense list" />
    <ul>
        {#each expenses as expense, index}
        <Expense {...expense} />
        {:else}
        <h2>there are no expanses currently</h2>
        {/each}
    </ul>
</section>