<script>
    import {setContext} from "svelte";
    import {writable} from "svelte/store";
    import CounterUsingStoreInContext from "./store/counterUsingStore.svelte";
    import DisplayCounterUsingStore from "./store/displayCounterUsingStore.svelte";

    const contextStore = writable({counterValue: 0})
    setContext('counterContextUsingStore', contextStore)
</script>

<div class="counter-container">
    <h2 class="counter-title">This is a counter using a store in a context to spread the counter value over children components, and share the update using the store !</h2>
    <CounterUsingStoreInContext/>
    <DisplayCounterUsingStore/>
</div>

