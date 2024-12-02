<script>
    import {getContext} from 'svelte';

    const counterUsingStoreContext = getContext('counterContextUsingStore')

</script>

<div>
    {#each {length: $counterUsingStoreContext.counterValue} as _,i}
        <p>looping for {i+1} counter value</p>
    {/each}
</div>

<style>
    p {
        font-size: 1.2rem;
        color: #1C5588;
        margin-top: 20px;
    }
</style>