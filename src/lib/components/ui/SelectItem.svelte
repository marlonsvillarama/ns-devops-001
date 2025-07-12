<script>
    let {
        text = ''
    } = $props();
</script>

<button>{text}</button>

<style>
    button {
        background-color: var(--bg-lighter);
        color: var(--text-dark);
        cursor: pointer;
        font-size: var(--text-xl);
        padding: 0.375rem 1rem;
    }
    button:hover {
        background-color: var(--bg-light);
    }
</style>