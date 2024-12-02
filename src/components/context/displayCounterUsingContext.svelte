<script>
    import {getContext} from 'svelte';

    const counterContext = getContext('counterContext')
</script>

<div>
    <p>{counterContext.counterValue}</p>
</div>

<style>
    p {
        font-size: 1.2rem;
        color: #1C5588;
        margin-top: 20px;
    }
</style>