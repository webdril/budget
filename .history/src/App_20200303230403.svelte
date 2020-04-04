<script>
import {setContext} from 'svelte';
// components
import Navbar from './Navbar.svelte'
import ExpensesList from './ExpensesList.svelte'

// Data
import expensesData from './expenses';

// variables
let expenses = [...expensesData];

// functions
function removeExpense(id){
	expenses = expenses.filter(item =>item.id !== id);
}

// context
setContext('remove', removeExpense)
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<main class="content">
	<ExpensesList {expenses}/>
</main>
