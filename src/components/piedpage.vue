<script>
export default {
    name: 'foo-ter',
}
</script>

<template>
    <div class="footer">
        <div class="menulogo"><a href="#/"><img class="logo" alt="Vue logo" src="../assets/navbar/Lakson-logo.png"></a>
        </div>
        <div class="menu">All rights reserved.</div>
    </div>
</template>

<style>
.footer {
    background-color: #CD2428;
    border: 1px solid #FAF5D0;
    height: 3.5rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    /* margin: 1rem; */
    color: #FAF5D0;
    font-size: 1.2rem;
    font-family: 'Cormorant Garamond', serif;
    font-weight: 100;
}
.menu {
    display: flex;
    justify-content: right;
    padding-right: 1rem;
}
</style>