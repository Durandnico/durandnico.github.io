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
    background-color: #1e1f26;
    display: flex;
    flex-direction: column;
}


.mypadding {
    position: relative;
    min-height: 64px;
}

footer {
    position: absolute;
    bottom: 40px;
    right:25px;
    z-index: 100;
    color:white;
}
</style>