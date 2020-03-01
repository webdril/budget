<script>
import Navbar from './Navbar.svelte'
import expensesData from './expenses';
let expenses = [...expensesData];
console.log(expenses);
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<Title title="add expense"/>
<Title title="expense list"/>

