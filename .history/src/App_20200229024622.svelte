<script>
import Navbar from './Navbar.svelte'
import Title from './Title.svelte'
let fruits = ['apple', 'orange', 'lemon']
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<Title title="add expense"/>
<Title title="expense list"/>

{#each fruits as item}

<Title title= {item}/>
{/each}