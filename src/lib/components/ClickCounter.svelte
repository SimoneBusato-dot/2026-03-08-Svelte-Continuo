<script>
    let props = $props()
    let count = $state(props.initialCount || 0)
    let double = $derived(count*2)
</script>

<button onclick={() => count++}>
    Clicks: {count}
</button>
<span> doubled is {double}</span>


