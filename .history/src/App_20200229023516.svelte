<script>
import Navbar from './Navbar.svelte'
import Title from './Title.svelte'
import Example from './Example.svelte'
let fruits = ['apple', 'orange', 'lemon']
</script> 

<!-- CSS/STYLING -->

<Navbar /> 
<Title title="add expense"/>
<Title title="expense list"/>

{#each fruits as item}
<h1>default title</h1>
{/each}