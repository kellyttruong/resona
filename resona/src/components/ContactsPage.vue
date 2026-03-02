<script setup></script>

<template>

<body>
    <header>
        <h3 class="rubik">contact</h3>
    </header>
    <img src="../assets/television.png" alt id="tv"><video src=""></video>
    <footer>
        <a href=""><img src="../assets/ig-logo.png" alt id="ig"></a>
        <div class="help">
            <p class="lexend" id="title">Helpful Links</p>
            <a href="" class="lexend">BPM festival</a>
            <br>
            <a href="" class="lexend">Presentation</a>
        </div>
        <div class="about">
            <p class="lexend" id="title">About us</p>
            <a href="https://582multi.media/" class="lexend">Contact us</a>
            <br>
            <a href="https://www.figma.com/design/h0LYGmI8g1IcsFRQilUHML/Capython-2026?node-id=0-1&t=8Ysswi7g8F5GYdgE-1" class="lexend">Figma</a>
        </div>
        <p class="lexend">&copy;2026 Resona</p>
    </footer>
</body>

</template>

<style lang="scss" scoped>
#tv {
    grid-column: span 2;
    text-align: center;
    width: 300px;
}

#title {
    font-weight: 600px;
}

footer {
    grid-column: span 2;
    text-align: center;
    margin-top: 10px;
    background-color: #8f0410;
}

a, p {
    color: white;
    text-decoration: none;
}
</style>
