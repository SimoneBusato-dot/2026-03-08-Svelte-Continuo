<script>
    let {initialCount: count = $bindable()} = $props()
    
    let double = $derived(count*2)
</script>

<button onclick={() => count++}>
    Clicks: {count}
</button>
<span> doubled is {double}</span>



