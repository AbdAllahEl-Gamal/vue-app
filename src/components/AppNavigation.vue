<template>
    <div>
        <div class="row nav-section">
            <div class="nav-left-icon col-6">
                <img src="365LogoFinalWhite1.png">                
            </div>
            <div class="nav-right col-6">
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
    computed: {
    },
    methods: {
    }
};
</script>

<style scoped>
.nav-section {
    padding-top: 45px;
}

.nav-left-icon {
    padding-left: 133px;
}

.navbar-light .navbar-nav .nav-item {
    padding-right: 10px;
    padding-left: 10px;
}

.navbar-light .navbar-nav .nav-link {
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    color: #FFFFFF;
}

.login-btn {
    border: 2px solid;
}
</style>
