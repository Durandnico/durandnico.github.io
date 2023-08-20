<template>
    <div class="home">
        <section class="nav">
            <h1>Durand Nicolas</h1>
            <h3 class="span loader">
                <span class="m">C</span>
                <span class="m">o</span>
                <span class="m">d</span>
                <span class="m">i</span>
                <span class="m">n</span>
                <span class="m">g</span>
                <span class="m">&nbsp;</span>
                <span class="m">N</span>
                <span class="m">'</span>
                <span class="m">&nbsp;</span>
                <span class="m">R</span>
                <span class="m">u</span>
                <span class="m">n</span>
                <span class="m">n</span>
                <span class="m">i</span>
                <span class="m">n</span>
                <span class="m">g</span>
                <span class="m">&nbsp;</span>
                <span class="m">4</span>
                <span class="m">&nbsp;</span>
                <span class="m">L</span>
                <span class="m">i</span>
                <span class="m">f</span>
                <span class="m">e</span>
            </h3>
        </section>
    </div>
</template>




<style scoped>

.home {
    position: absolute;
    width: 100vw;
    font-family: "ROBOTO", sans-serif;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

.nav {
  position: absolute;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 93.14vh;
  width: 100vw;
  background-color: #1e1f26;
  text-align: center;
  padding: 0 2em;
}

.nav h1,
.slider h1 {
  font-family: "Josefin Sans", sans-serif;
  font-size: 5vw;
  margin: 0;
  padding-bottom: 0.5rem;
  letter-spacing: 0.5rem;
  color: #03dac6;
  transition: all 0.3s ease;
  z-index: 3;
}
h1:hover {
  transform: translate3d(0, -10px, 22px);
  color: #ff0266;
}

h3.span {
  font-size: 2vw;
  letter-spacing: 0.7em;
  font-family: "ROBOTO", sans-serif;
  font-weight: 300;
  color: #faebd7;
  z-index: 4;
}
span:hover {
  color: #ff0266;
  font-weight: 500;
  font-size: 2.2vw;
}

a {
  text-decoration: none;
}

@media (min-width: 800px) {
  .nav h1,
  .slider h1 {
    font-size: 5vw;
  }

  .nav h2,
  .slider h2 {
    font-size: 3vw;
  }

  .nav-tab {
    font-size: 3vw;
  }
}

@media screen only (min-width: 360px) {
  .nav h1,
  .slider h1 {
    font-size: 8vw;
  }

  .nav h2,
  .slider h2 {
    font-size: 2vw;
    letter-spacing: 0.2vw;
  }

  .nav-tab {
    font-size: 1.2vw;
  }
}

.loader span {
  color: #faebd7;
  text-shadow: 0 0 0 #faebd7;
  -webkit-animation: loading 1s ease-in-out infinite alternate;
}

@-webkit-keyframes loading {
  to {
    text-shadow: 20px 0 70px #ff0266;
    color: #ff0266;
  }
}
.loader span:nth-child(2) {
  -webkit-animation-delay: 0.1s;
}
.loader span:nth-child(3) {
  -webkit-animation-delay: 0.2s;
}
.loader span:nth-child(4) {
  -webkit-animation-delay: 0.3s;
}
.loader span:nth-child(5) {
  -webkit-animation-delay: 0.4s;
}
.loader span:nth-child(6) {
  -webkit-animation-delay: 0.5s;
}
.loader span:nth-child(7) {
  -webkit-animation-delay: 0.6s;
}
.loader span:nth-child(8) {
  -webkit-animation-delay: 0.7s;
}
.loader span:nth-child(9) {
  -webkit-animation-delay: 0.8s;
}

.loader span:nth-child(10) {
  -webkit-animation-delay: 0.9s;
}
.loader span:nth-child(11) {
  -webkit-animation-delay: 1s;
}
.loader span:nth-child(12) {
  -webkit-animation-delay: 1.1s;
}
.loader span:nth-child(13) {
  -webkit-animation-delay: 1.2s;
}
.loader span:nth-child(14) {
  -webkit-animation-delay: 1.3s;
}
.loader span:nth-child(15) {
  -webkit-animation-delay: 1.4s;
}
.loader span:nth-child(16) {
  -webkit-animation-delay: 1.5s;
}
.loader span:nth-child(17) {
  -webkit-animation-delay: 1.6s;
}
.loader span:nth-child(18) {
  -webkit-animation-delay: 1.7s;
}
.loader span:nth-child(19) {
  -webkit-animation-delay: 1.8s;
}
.loader span:nth-child(20) {
  -webkit-animation-delay: 1.9s;
}
.loader span:nth-child(21) {
  -webkit-animation-delay: 2s;
}
.loader span:nth-child(22) {
  -webkit-animation-delay: 2.1s;
}

</style>


