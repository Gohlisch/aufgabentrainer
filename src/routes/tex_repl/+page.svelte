<script lang="ts">
    import TexEditor from "../../lib/shared_components/TexEditor.svelte";
    import ColorButton from "../../lib/shared_components/tex_editor/ColorButton.svelte";

    let formula: string;
	let selectionStart: number = 0;
	let selectionEnd: number = 0;

    function chooseColor(color: string) {
        formula = formula.slice(0, selectionStart)
                + color
                + formula.slice(selectionEnd);
    }
</script>

<style>
    .editor {
        width: 100vw;
    }
</style>
<section class="editor">
    <menu>
        <li>
            <ColorButton on:input={(e)=>chooseColor(e.detail.value)}></ColorButton>
        </li>
    </menu>
    <TexEditor bind:formula on:input={e=>{
        selectionStart = e.detail.selectionStart;
        selectionEnd = e.detail.selectionEnd;
    }}/>

</section>
