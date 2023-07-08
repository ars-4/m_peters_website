<template>
    <div class="navbar">
        <div class="brand">
            <h1>M</h1>
            <h3>Peters</h3>
        </div>
        <div class="navbar-links">
            <router-link to="/">Home</router-link>
            <router-link to="/gallery">Gallery</router-link>
            <router-link to="#">Contact</router-link>
        </div>
    </div>
</template>

<style>
.navbar {
    padding: 10px 15px;
    background-color: var(--bg-primary);
    color: var(--text-secondary);
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}

.navbar .brand {
    display: flex;
    justify-content: center;
    align-items: center;
}

.navbar .navbar-links a {
    padding: 0px 15px;
}

@media screen and (max-width : 700px) {
    .navbar .brand h3 {
        font-size: 16px;
    }
    .navbar .brand {
        text-align: left;
        justify-content: left;
    }
    .navbar-links,
    .navbar-links a {
        padding-left: 0px !important;
    }
}
</style>