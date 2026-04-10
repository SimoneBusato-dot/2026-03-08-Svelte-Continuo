<script>
    import {website} from "$lib/state.svelte"
    import ClickCounter from "$lib/components/ClickCounter.svelte";
    import CanvasSquare from "$lib/components/CanvasSquare.svelte";
    import ToDoList from "$lib/components/ToDoList.svelte";
    import TitleEditor from "$lib/components/TitleEditor.svelte";

    let count = $state(5)
</script>

<TitleEditor />

<h1>{website.title}</h1>

<ClickCounter bind:initialCount={count}/>

{#if count >= 10 && count <= 20}
    <p>count form parent is {count}</p> 
    {:else if count >= 30}
    <p>too many clicks!!</p>
    {:else}
    <p>count is not in range</p>
{/if}

<CanvasSquare />

<ToDoList />

