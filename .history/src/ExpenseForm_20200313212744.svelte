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
        <div class="form-control">
            <label for="amount">amount</label>
            <input type="number" id="amount" />
        </div>
        <p class="form-empty">Please fill out all form field</p>
        <button type="submit" class="btn btn-block">add expense</button>
        <button type="button" class="close-btn">
        <i class="fas fa-times" / >close
        </button>
    </form>
</section>