<template>
    <v-app>
        <header>
            <Navbar />
        </header>

        <div class="main">
            <div class="mypadding"></div>
            <slot />
        </div>
        
        <footer>
            <SocialMedia class="hidden-lg-and-up" />
        </footer>
    </v-app>
</template>


<style>


.main {
    position: absolute;
    width: 100vw;
    min-height: 100vh;
    top:0;
    font-family: "ROBOTO", sans-serif;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    color: white;
    background-color: #363a4f;
    display: flex;
    flex-direction: column;
}


.mypadding {
    position: relative;
    min-height: 64px;
}

footer {
    position:fixed;
    bottom: 40px;
    right:25px;
    z-index: 100;
}
</style>