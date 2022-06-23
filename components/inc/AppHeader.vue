<template>


        
        <nav>
            <a href="#" class="nav-icon" aria-label="visiter page d'accueil" aria-current="page">
                <img src="~/assets/logo.png" alt="logo">
                <span>Le Corps Pilates</span>
            </a>
            <div class="main-navlinks">
                <button class="hamburger" type="button" aria-label="Toggle navigation" aria-expanded="false">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
            </div>
            <div class="navlinks-container">
                <a href="#" aria-current="page">Accueil</a>
                <a href="#">Présentation</a>
                <a href="#">Pilates</a>
                <a href="#">Horaires & Tarifs</a>
                <a href="#">Contact</a>
            </div>
            <div class="nav-reseaux">
                <a href="#"><font-awesome-icon icon="fa-brands fa-facebook-f" /></a>
                <a href="#"><font-awesome-icon icon="fa-brands fa-instagram" /></a>
            </div>

        </nav>


</template>


<script>
export default {
  name: 'AppHeader'
}
</script>


<style lang="scss" scoped>
::before,
::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Montserrat,Helvetica,sans-serif;
    background: #f4f4f4;
}
nav {
    position: fixed;
    width: 100%;
    display: flex;
    align-items: center;
    padding: 15px 25px;
    background: #fafafa;
    box-shadow: inset 0px -1px 0px #c5c5c6;
}
.nav-icon {
    display: flex;
    align-items: center;
    text-decoration: none;
    margin-right: 20px;
}
.nav-icon span {
    font-family: Roboto Flex, sans-serif;
    font-size: 25px;
    margin-left: 10px;
    font-weight: 400;
    color: #333;
}
.nav-icon img {
    width: 40px;
}
.hamburger {
    display: none;
}
.navlinks-container a {
    margin: 0 10px;
    font-size: 16px;
    font-weight: 500;
    text-decoration: none;
    color:#333;
    display: inline-block;
    position: relative;
}
img {
    width: 20px;
}
</style>