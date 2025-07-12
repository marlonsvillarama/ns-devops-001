<script>
    import '$lib/style/app.css';
    import Button from "$lib/components/ui/Button.svelte";
    import Input from '$lib/components/ui/Input.svelte';
    import Select from '$lib/components/ui/Select.svelte';
    import SelectItem from '$lib/components/ui/SelectItem.svelte';
</script>

<main>
    <Button>Create new field</Button>
    <Input layout="row" placeholder="test" />
    <Select label="Select an option...">
        <SelectItem>Option 1</SelectItem>
        <SelectItem>Option 2</SelectItem>
        <SelectItem>Option 3</SelectItem>
    </Select>
</main>

<style>
    main {
        padding: 1rem;
    }
</style>