<script>
    import {getContext} from 'svelte';

    const counterContext = getContext('counterContext')
    $: counterValue = counterContext.counterValue
</script>

<div>
    <button class="counter-button"
            onclick={() => counterContext.counterValue++}
    >
        Click me ! {counterValue > 0 && `(${counterValue})`}
    </button>
</div>
