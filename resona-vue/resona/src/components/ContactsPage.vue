<script setup></script>

<template>



    <div class="app-container">
    <header>
        <h3 class="rubik">contact</h3>
    </header>
        <img id="tv" src="../assets/television.png" alt=""> <!-- <video src=""></video> /-->
    </div>

    <footer class="app-container">
        <a href=""><img src="../assets/ig-logo.png" alt id="ig"></a>
        
        <div class="help">
            <p class="lexend" id="title">Helpful Links</p>
            <a href="https://bpm.capython.com/" class="lexend">BPM festival</a>
            <br>
            <a href="" class="lexend">Presentation</a>
        </div>

        <div class="about">
            <p class="lexend" id="title">About us</p>
            <a href="https://582multi.media/" class="lexend">Contact us</a>
            <br>
            <a href="https://www.figma.com/design/h0LYGmI8g1IcsFRQilUHML/Capython-2026?node-id=0-1&t=8Ysswi7g8F5GYdgE-1" class="lexend">Figma</a>
        </div>

        <p class="lexend" id="copy">&copy;2026 Resona</p>

        <img src="../assets/wHITE VERSION.png" alt id="logo">
    </footer>

</template>

<style lang="scss" scoped>

header {
    grid-column: 3;
}

#tv {
    grid-column: span 3;
    justify-self: center;
    width: 550px;
    max-width: 100%;
    padding: 50px;
}

#title {
    font-weight: bold;
}

a.lexend {
    font-weight: 250;
}

footer {
    grid-column: span 2;
    margin-top: 10px;
    background-color: #8f0410;
    padding: 20px;
}

a, p {
    color: white;
    text-decoration: none;
}

#copy {
    grid-row: 2;
    grid-column: 2;
    text-align: center;
}

div .help {
    // padding: 20px;
    text-align: right;
}

div .about {
    // padding: 20px;
    text-align: right;
}

#logo {
    width: 110px;
    grid-column: 3;
    justify-self: right;
}

.app-container {
    height: auto;
    grid-template-rows: 1fr;
    grid-template-columns: repeat(3, 1fr);
}
 
@media screen and (min-width: 1080px) {
      .app-container {
        grid-template-columns: repeat(5, 1fr);
        padding: 10px;
    }

    #tv {
        grid-column: 3;
        grid-column: span 5;
        width: 700px;
    }
    
    header {
        grid-column: 5;
    }

    .help {
      grid-column: 4;  
    }

    .about {
        grid-column: 5;
    }

    #copy {
        grid-column: 1;
        justify-self: left;
        position: fixed;
        bottom: 0;
        margin-bottom: 10px;
    }

    #logo {
        grid-column: 5;
        width: 200px;
    }
}

</style>
