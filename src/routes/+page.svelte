<script>
    import ClickCounter from "$lib/components/ClickCounter.svelte";
    import CanvasSquare from "$lib/components/CanvasSquare.svelte";

    let count = $state(5)
</script>

<ClickCounter bind:initialCount={count}/>
<p>count form parent is {count}</p>
<CanvasSquare />

