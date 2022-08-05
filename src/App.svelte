<script>
    //components
    import Navbar from './Navbar.svelte';
    import ExpensesList from './ExpensesList.svelte';
    import Expense from './Expense.svelte';
    //data
    import expensesData from './expenses'
    //variables
    let expenses =[...expensesData];
</script>

<style>
    h2{ text-transform: capitalize;}
</style>

<Navbar />
<main class="content">
    <ExpensesList {expenses} />
</main>
