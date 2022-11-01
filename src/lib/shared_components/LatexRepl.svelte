<script lang="ts">
	import Formula from "./Formula.svelte";

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
    <Formula formula={formula}></Formula>
</article>
