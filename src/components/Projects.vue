<template>
    <div class="container">
        <h1>Projects</h1>
        <div class="grid">
            <div class="grid-cell">
                Cell 1
            </div>
            <div class="grid-cell">
                Cell 2
            </div>
            <div class="grid-cell">
                Cell 2
            </div>
            <div class="grid-cell">
                Cell 3
            </div>
        </div>
    </div>
</template>
<style scoped>
h1 {
    font-family: "Comic Sans MS", "Comic Sans", cursive;
}

.container {
    margin-bottom: 100px;
    width: 60%;
    
    margin-left:auto;
    margin-right:auto;

}

.grid {
    display: grid;
    justify-content: start;
    grid-template-columns: 50% 50%;
    grid-template-rows: 50% 50%;
    grid-row-gap: 1px;
    grid-column-gap: 1px;
}

.grid-cell {
    background-color: #F3C;
}

</style>