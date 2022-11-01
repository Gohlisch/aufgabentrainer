<script lang="ts">
	import FormularRenderer from "./FormularRenderer.svelte";

	export let formula: string = "";
</script>

<style>
    article {
        display: grid;
        grid-template-columns: [input] 50% [rendered_formulars] 50%
    }

    textarea {
        resize: none;
    }
</style>

<article>
    <textarea bind:value={formula}></textarea>
    <FormularRenderer formula={formula}></FormularRenderer>
</article>
