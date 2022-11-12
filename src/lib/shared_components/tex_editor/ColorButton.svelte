<script lang="ts">
    import {createEventDispatcher} from "svelte";

    const dispatch : ((name: string, detail?: any) => void) = createEventDispatcher();
	let menuClosed = true;

	function propagateValueAndCloseMenu(value: string) {
		dispatch("input", {value: ` \\color\{${value}\} `});
		menuClosed = true;
    }
import PopUpButtonMenu from "../PopUpButtonMenu.svelte";
</script>

<PopUpButtonMenu bind:menuClosed={menuClosed}>
    <span>\color{"{"}</span>
    <select on:input|stopPropagation ={e => propagateValueAndCloseMenu(e.target.value)}>
        <option value="Apricot">Apricot</option>
        <option value="Blue">Blue</option>
        <option value="Brown">Brown</option>
        <option value="Cerulean">Cerulean</option>
        <option value="DarkOrchid">DarkOrchid</option>
        <option value="Goldenrod">Goldenrod</option>
        <option value="JungleGreen">JungleGreen</option>
        <option value="Mahogany">Mahogany</option>
        <option value="Mulberry">Mulberry</option>
        <option value="OrangeRed">PineGreen</option>
        <option value="PineGreen">PineGreen</option>
        <option value="RawSienna">RawSienna</option>
        <option value="Rhodamine">Rhodamine</option>
        <option value="Salmone">Salmone</option>
    </select>
    <span>{"}"}</span>
</PopUpButtonMenu>
