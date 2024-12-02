<script>
    import {setContext} from "svelte";
    import CounterUsingContext from "./context/counterUsingContext.svelte";
    import DisplayCounter from "./context/displayCounterUsingContext.svelte";
    import '../styles/general.css';

    setContext('counterContext', {counterValue:3});
</script>

<div class="counter-container">
    <h2 class="counter-title">This is a stupid counter with a context to share the counter value over children components, but it does not share the update !</h2>
    <CounterUsingContext/>
    <DisplayCounter/>
</div>

