<script>
    import Counter from "../components/counter.svelte";
    import DumbDisplay from "../components/dumbDisplay.svelte";
    import CounterWithContext from "../components/counterWithContext.svelte";
    import CounterWithStore from "../components/counterWithStore.svelte";

    const props = 'tchoupi'
</script>

<main>
    <Counter/>
    <DumbDisplay {props}/>
    <CounterWithContext/>
    <CounterWithStore/>
</main>