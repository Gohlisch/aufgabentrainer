<script lang="ts">
    export let formula: string = "";
</script>

<style>
    article {
        background-color: white;
    }
</style>

<article>
    <la-tex display="block" {formula}>{formula}</la-tex>
</article>
