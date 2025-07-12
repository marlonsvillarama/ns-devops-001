<script>
    let {
        children,
        defaultText = '',
        label = ''
    } = $props();
    let id = `popover-${new Date().getTime()}`;
</script>

<button popovertarget={id}>{label}</button>
<div class="popover" {id} popover>{@render children?.()}</div>

<style>
    button {
        background-color: var(--bg-light);
        border: 1px solid var(--border);
        border-radius: var(--radius);
        color: var(--text-dark);
        cursor: pointer;
        font-size: var(--text-xs);
        font-weight: 500;
        /* letter-spacing: 0.25px; */
        padding: 0.5rem 1rem;
    }
    .popover {
        border: 1px solid var(--border);
        border-radius: 0.375rem;
    }
</style>