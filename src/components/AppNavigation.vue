<template>
    <div>
        <div class="row nav-section">
            <div class="nav-left-icon col-5">
                <img src="365LogoFinalWhite1.png">                
            </div>
            <div class="nav-right col-7">
                <nav class="navbar navbar-expand-lg navbar-light">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About us</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">How it works</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Blog</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact</a>
                        </li>
                        <li class="nav-item login-btn">
                            <a class="nav-link" href="#">Login</a>
                        </li>
                    </ul>
                </nav>
            </div> 
        </div>      
    </div>
</template>

<script>
export default {
    name: 'AppNavigation',
    data() {
        return {
            items: [
                { title: 'Home', url: '/' },
                { title: 'About us', url: '/aboutUs' },
                { title: 'How it works', url: '/howItWorks' },
                { title: 'Blog', url: '/blog' },
                { title: 'Contact', url: '/contact' },
                { title: 'Login', url: '/login' }
            ]
        };
    },
    methods: {
    }
};
</script>

<style scoped>
.nav-section {
    padding-top: 45px;
    padding-bottom: 65px;
}

.nav-left-icon {
    padding-left: 115px;
}

.navbar-light .navbar-nav .nav-item a {
    cursor: pointer;
}

.navbar-light .navbar-nav .nav-item {
    padding-right: 20px;
}

.navbar-light .navbar-nav .nav-link {
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
}

.login-btn {
    position: relative;
    cursor: pointer;
    max-width: 250px;
    color: #ffffff;
    border-style: solid;
    border-width: 2px;
    border-image: linear-gradient(220deg, #9672FF 27.76%, rgba(107, 79, 232, 0) 94.18%) 1;
    clip-path: polygon(0 0, 90% 0, 100% 26%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    padding-right: 25px;
    padding-left: 25px;
}

.login-btn:hover {
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
}

.login-btn:before {
    position: absolute;
    content: "";
    z-index: -1;
    top: -1px;
    right: -15px;
    bottom: 0;
    -webkit-mask: linear-gradient(#ffffff 0 0) content-box, linear-gradient(#ffffff 0 0);
    mask: linear-gradient(#ffffff 0 0) content-box, linear-gradient(#ffffff 0 0);
    -webkit-mask-composite: xor;
    mask-composite: exclude;
    border-right: 3px solid #9672FF;
    transform: skew(+45deg);
}

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  .nav-section {
    padding-bottom: 30px;
  }
  .navbar-nav {
    display: contents;
  }
  .nav-left-icon {
    padding-left: 20px;
  }
  .navbar-light .navbar-nav .nav-item {
    padding-right: 20px;
  }
  .nav-right {
    width: auto;
  }
}
</style>
