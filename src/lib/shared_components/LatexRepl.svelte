<script lang="ts">
	import FormulaRenderer from "./FormulaRenderer.svelte";

	export let formula: string = "";
</script>

<style>
    article {
        display: grid;
        grid-template-columns: [input] 50% [rendered_formulars] 50%;
        background-color: white;
    }

    textarea {
        resize: none;
    }
</style>

<article>
    <textarea bind:value={formula}></textarea>
    <FormulaRenderer formula={formula}></FormulaRenderer>
</article>
