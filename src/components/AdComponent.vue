<template>
    <div class="ad-box">
        <div class="box">
            <span>ADVERTISEMENT</span>
        </div>
    </div>
</template>

<style>

.ad-box {
    border-radius: 4px;
    overflow: hidden;
    width: 100%;
    aspect-ratio: 1/2;
    border: 1px solid #c3c3c3;
    cursor: pointer;
    margin: 10px 4px;
}

.ad-box .box {
    width: 100%;
    height: 100%;
    text-align: center;
    justify-content: center;
    align-items: center;
    color: #c3c3c3;
    display: flex;
    transition: 0.5s;
}

@media screen and (max-width:700px) {
    .ad-box {
        aspect-ratio: 4/2;
    }
    .pc-only {
        display: none;
    }
}
</style>