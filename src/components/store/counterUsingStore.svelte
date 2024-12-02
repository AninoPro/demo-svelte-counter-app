<script>
    import {getContext} from 'svelte';

    const counterUsingStore = getContext('counterContextUsingStore')
</script>

<div>
    <button class="counter-button"
            onclick={() => $counterUsingStore.counterValue++}
    >
        Click me ! {#if $counterUsingStore.counterValue > 0}({$counterUsingStore.counterValue}){/if}
    </button>
</div>
