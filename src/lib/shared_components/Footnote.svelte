<script lang="ts">
    export let link;
	export let number;
</script>

<script context="module">
    export let ascendingNumber = 0;
</script>

<style>
    a {
        font-size: 0.5em;
    }
</style>

<a href={link}>{number || ++ascendingNumber}</a>
