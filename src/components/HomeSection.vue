<template>
    <!-- start Home Section -->
    <div id="home">
        <!-- Start navigation -->
        <nav class="navbar navbar-expand-md navbar-dark bg-dark fixed-top">
            <a href="#home" class="navbar-brand">
                <img src="@/assets//images/logo.png" alt="Toptal-Network" />
                <div>Toptal Network</div>
            </a>
            <button
                type="button"
                class="navbar-toggler"
                data-toggle="collapse"
                data-target="#navbarResponsive"
            >
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collpase navbar-collapse" id="navbarResponsive">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item">
                        <a href="#home" class="nav-link">Home</a>
                    </li>
                    <li class="nav-item">
                        <a href="#ourGoal"  class="nav-link">Our Goal</a>
                    </li>
                    <li class="nav-item">
                        <a href="#events"  class="nav-link">Events</a>
                    </li>
                    <li class="nav-item">
                        <a href="#contact"  class="nav-link">Contact</a>
                    </li>
                </ul>
            </div>
        </nav>
        <!-- End navigation -->

        <!-- Start Hero -->
        <div class="hero home-hero">
            <div class="overlay"></div>
        </div>
        <div class="caption text-center">
            <div class="header">Welcome To Toptal Network</div>
            <div class="subheader">Your personal guide to remote work</div>
            <a
                href="https://t.me/+FhvGOWeRdQI2NGM0"
                target="_blank"
                class="btn btn-outline-light btn-lg"
            >
                Join our Telegram chat
            </a>
        </div>
        <!-- End Hero -->
    </div>
    <!-- end Home Section -->
</template>

<script>
export default {
    name: "home",
    mounted(){
        location.href = "/#home"
    }
};
</script>
<style scoped>
.navbar {
    text-transform: uppercase;
    font-weight: 700;
    font-size: 0.9rem;
    letter-spacing: 0.1rem;
    background-color: rgba(0, 0, 0, 0.7) !important;
}
.navbar-brand {
    display: flex;
    align-items: center;
}
.navbar-brand img {
    border-radius: 100%;
    margin-right: 10px;
    height: 2rem;
}
.navbar-toggler {
    outline: none !important;
}
.navbar-nav li {
    padding-right: 0.5rem;
}
.navbar .navbar-nav .nav-link {
    color: white;
    padding-top: 0.8rem;
}
.navbar .navbar-nav .nav-link.active,
.navbar .navbar-nav .nav-link:hover {
    color: #204ecf;
    cursor: pointer;
}
.header {
    font-size: 4rem;
}
.subheader {
    font-size: 2.5rem;
    margin-bottom: 20px;
}
@media only screen and (max-width: 700px) {
    .header {
        font-size: 2.5rem;
    }
    .subheader {
        font-size: 1.5rem;
        margin-bottom: 20px;
    }
}
.hero {
    height: 100vh;
    width: 100%;
    position: relative;
}
.hero .overlay {
    position: absolute;
    top: 0;
    height: 100vh;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.7);
}
.home-hero {
    background-image: url("../assets/images/home-bg.jpg");
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.caption {
    position: absolute;
    top: 35%;
    width: 100%;
    color: white;
    text-transform: uppercase;
}
.caption h1 {
    font-size: 3.8rem;
    font-weight: bold;
    letter-spacing: 0.3rem;
    text-shadow: 0.1rem 0.1rem 0.8rem black;
    padding-bottom: 1rem;
}
.caption h3 {
    font-size: 2rem;
    text-shadow: 0.1rem 0.1rem 0.8rem black;
    padding-bottom: 1rem;
}
</style>
