<div class="mainContainer">
    <slot/>
</div>

<style>
    .mainContainer {
        min-height: 100vh;
        background: linear-gradient(to right, #002804, #004600);
        color: white;
        position: relative;
        display: flex;
        flex-direction: column;
    }
</style>