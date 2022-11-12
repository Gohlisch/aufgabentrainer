<script lang="ts">
    export let menuClosed: boolean = true;
</script>
<style>
    .menuClosed {
        display: none;
    }
</style>
<button on:click={()=> menuClosed = !menuClosed}>
</button>
<div class:menuClosed>
    <slot></slot>
</div>
