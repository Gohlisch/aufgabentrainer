<script lang="ts">
	import Formula from "./Formula.svelte";
	import {createEventDispatcher} from "svelte";

	export let formula: string = "";

	const dispatch : ((name: string, detail?: any) => void) = createEventDispatcher();

	function propagate(value: string, selectionStart: number, selectionEnd: number) {
		dispatch("input", {value, selectionStart, selectionEnd});
	}
</script>

<style>
    article {
        display: grid;
        grid-template-columns: [input] 50% [rendered_formulars] 50%;
        background-color: white;
        width: 100vw
    }

    textarea {
        resize: none;
    }
</style>

<article>
    <textarea bind:value={formula} on:input={(e)=>propagate(e.target.value, e.target.selectionStart, e.target.selectionEnd)}></textarea>
    <Formula formula={formula}></Formula>
</article>
