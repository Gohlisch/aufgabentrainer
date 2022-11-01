<script>
    import Header from "../lib/shared_components/Header.svelte";
</script>

<style>
    main {
        max-width: 20cm;
        min-width: 50%;
        padding: 0 1em;
    }
</style>

<Header></Header>
<main>
    <slot></slot>
</main>
<footer>

</footer>
