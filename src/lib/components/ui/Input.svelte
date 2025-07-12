<script>
    let {
        layout = 'col',
        label = '',
        placeholder = ''
    } = $props();
</script>

<div class={[
    "input",
    { "flex-col": layout === 'col' },
    { "flex-row": layout === 'row' }
]}>
    {#if label}
        <span>{label}</span>
    {/if}
    <input type="text" {placeholder} />
</div>

<style>
    .input {
        align-items: center;
        color: var(--text-darker);
        font-size: var(--text-sm);
        gap: 0.5rem;
    }
    span {
        font-weight: 500;
    }
    input[type=text] {
        border: 1px solid var(--border);
        border-radius: var(--radius-sm);
        font-size: var(--text-sm);
        min-width: 20rem;
        width: 20rem;
        padding: 0.5rem 0.75rem;
    }
</style>