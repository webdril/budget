<script>
import Navbar from './Navbar.svelte'
import Title from './Title.svelte'
import Example from './Example.svelte'
</script> 

<style>
	span{
		background: green;
		color: blue;
	}
</style>
<!-- CSS/STYLING -->

<Navbar /> 
<Title title="add expense"/>
<Title title="expense list"/>
<Title />
<Example />