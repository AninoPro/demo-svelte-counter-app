<script>
    let count = 0
    let count2 = 0

    $: double = (() => {
        console.log("double recalculé !")
        return (count * 2)
    })()
</script>

<div class="counter-container">
    <h2 class="counter-title">This is a stoupid counter with a basic state management of the counter value</h2>
    <button
            class="counter-button"
            onclick={() => count++}
    >
        Count is {count} and double is {double}
    </button>
    <button
    class="counter-button"
    onclick={() => count2++}>
        Count2 is {count2}
    </button>
</div>

<style>
    @import '../styles/general.css';
</style>