<script>
    import Header from "../lib/shared_components/Header.svelte";
</script>

<style>
    main {
        max-width: 1000px;
        min-width: 50%;
    }
</style>

<Header></Header>
<main>
    <slot></slot>
</main>
