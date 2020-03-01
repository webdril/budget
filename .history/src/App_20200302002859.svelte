<script>
// components
import Navbar from './Navbar.svelte'
import ExpensesList from './ExpensesList.svelte'

// Data
import expensesData from './expenses';

// variables
let expenses = [...expensesData];
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<main class="content">
	<ExpensesList expenses={expenses}/>
</main>
