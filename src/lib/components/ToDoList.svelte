<script>
    let todos = $state([
        {title: "Assignment 1", done: false},
        {title: "Assignment 2", done: false},
        {title: "Assignment 3", done: false}
    ])
</script>

<ul>
    {#each todos as todo}
    <li>
        {todo.title}
        <input type="checkbox" bind:checked={todo.done}>
    </li>
    {/each}
</ul>