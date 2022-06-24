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
    color: $primary-color;
    display: inline-block;
    position: relative;
}
.navlinks-container a::after {
    content: "";
    display: block;
    position: absolute;
    bottom: -3px;
    width: 100%;
    height: 1px;
    transform: scaleX(0);
    transform-origin: left;
    background: $primary-color;
    transition: transform 0.3s ease-out;
}
.navlinks-container a:hover::after {
    transform: scaleX(1);
}
.nav-reseaux {
    margin-left: auto;

}

@media (max-width:900px) {
    nav {
        padding: 15px 20px;
        position: relative;
    }
    .nav-icon {
        order: 2;
        margin: 0 auto;
    }
    .nav-icon span {
        font-size: 22px;
    }
    .main-navlinks {
        order: 1;
    }
    /* Hamburger */
    .navlinks-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        position: absolute;
        background: #fafafa;
        top: 100%;
        left: 0;
        height: 100vh;
        border-right: 1px solid #c5c5c6;
    }
    .nav-reseaux {
        order: 3;
    }
}


img {
    width: 20px;
}
</style>