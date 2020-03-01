<script>
// components
import Navbar from './Navbar.svelte'
import ExpenseList from './ExpenseList'
// Data
import expensesData from './expenses';
// variables
let expenses = [...expensesData];
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<main class="content">
	<ExpenseList />
</main>
