<style>
    div::-webkit-scrollbar {
        display: none;
    }

    div {
        overflow-x: scroll;
        -ms-overflow-style: none;  /* IE and Edge */
        scrollbar-width: none;  /* Firefox */
        max-width: 100%;
    }
</style>
<div>
    <slot></slot>
</div>
