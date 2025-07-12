<script>
    let {
        children
    } = $props();
</script>

<button>
    {@render children?.()}
</button>

<style>
    button {
        background-color: var(--bg-dark);
        border: 1px solid transparent;
        border-radius: var(--radius);
        color: var(--text-lightest);
        cursor: pointer;
        font-size: var(--text-xs);
        font-weight: 500;
        /* letter-spacing: 0.25px; */
        padding: 0.5rem 1rem;
    }
    button:active {
        transform: translateY(1px);
    }
    button:hover {
        background-color: var(--bg-darker);
    }
</style>