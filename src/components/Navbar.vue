<template>
    <nav class="navbar is-primary" role="navigation" aria-label="main navigation">
        <div class="container">
            <div class="navbar-brand">
                <a class="navbar-item" href="/">
                    <div><i class="fas fa-language fa-2x" style="color:white;"></i></div>
                </a>

                <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                    <span aria-hidden="true"></span>
                </a>
            </div>

            <div id="navbarBasicExample" class="navbar-menu">
                <div class="navbar-start">
                    <a class="navbar-item" href="/">
                        Translator
                    </a>

                    <a class="navbar-item" href="about">
                        About
                    </a>

                    <div class="navbar-item has-dropdown is-hoverable">
                        <a class="navbar-link is-arrowless">
                            View on Github
                        </a>

                        <div class="navbar-dropdown">
                            <a class="navbar-item" href="https://github.com/MrMonk3y/Boopa-Dee-Bappa-Dee" target="_blank">
                                C Interpreter
                            </a>
                            <a class="navbar-item" href="https://github.com/b2a3e8/boopa-dee-bappa-dee.js" target="_blank">
                                JS Interpreter
                            </a>
                            <a class="navbar-item" href="https://github.com/b2a3e8/boopa-dee-bappa-dee.html" target="_blank">
                                This website
                            </a>
                        </div>
                    </div>
                </div>

                <!--<div class="navbar-end">
                    <div class="navbar-item">
                        <div class="buttons">
                            <a class="button is-primary">
                                <strong>Sign up</strong>
                            </a>
                            <a class="button is-light">
                                Log in
                            </a>
                        </div>
                    </div>
                </div>-->
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'Navbar',
    }
</script>
