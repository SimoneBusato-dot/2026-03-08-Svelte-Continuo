<script>
    import ClickCounter from "$lib/components/ClickCounter.svelte";

    let count = $state(5)
</script>

<ClickCounter bind:initialCount={count}/>

<p>count form parent is {count}</p>