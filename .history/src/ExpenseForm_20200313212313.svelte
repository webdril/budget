<script>
import Title from './Title.svelte'
</script>

<section class="form">
    <Title title= "add expense" />
    <form class="expense-form">
        <div class="form-control">
            <label for="name">Name</label>
            <input type="text" id="name" />
        </div>
    </form>
</section>