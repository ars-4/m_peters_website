<template>
    <div class="image-box">
        <div class="box">
            <span>IMAGE</span>
        </div>
    </div>
</template>

<style>

.image-box {
    border-radius: 4px;
    overflow: hidden;
    width: 100%;
    cursor: pointer;
    aspect-ratio: 12/13;
}
.image-box:hover .box {
    scale: 2;
    transition: 0.5s;
}

.image-box .box {
    width: 100%;
    height: 100%;
    background-color: #c3c3c3;
    text-align: center;
    justify-content: center;
    align-items: center;
    display: flex;
    transition: 0.5s;
}
</style>