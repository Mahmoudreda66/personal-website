<template>
    <header>
        <nav class="animate__animated animate__backInDown navbar navbar-expand-lg navbar-dark bg-transparent">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">Mahmoud Reda</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                    aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#features">Features</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#skills">Skills</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#projects">Projects</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#downloadCV">Download CV</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#personalInfo">Personal Info</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#contact">Contact Me</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
        <div style="margin-top: 100px;" class="animate__animated animate__backInLeft">
            <h1>Mahmoud Reda | <span>Backend Developer</span></h1>
            <p style="text-transform: capitalize; margin-bottom: 40px;">
                <span>i'm PHP developer, works with <i class="fab fa-laravel" style="color: #ff2718;"></i>
                    laravel</span><br><br>
                <span>fast learner, hard worker, efficient</span>
            </p>
            <button class="main" @click="scrollDown">Find More</button>
        </div>
        <div class="scroll-container animate__animated animate__backInUp">
            <div class="parent" @click="scrollDown">
                <span></span>
            </div>
        </div>
        <div class="icons animate__animated animate__backInRight">
            <ul>
                <li>
                    <a href="https://www.facebook.com/mahmoudreda66/" style="color: #fff;"><i
                            class="fab fa-facebook"></i></a>
                </li>
                <li>
                    <a href="https://www.linkedin.com/in/mahmoud-reda-616072256/" style="color: #fff;"><i
                            class="fab fa-linkedin"></i></a>
                </li>
                <li>
                    <a href="https://wa.me/+201274385491" style="color: #fff;"><i class="fab fa-whatsapp"></i></a>
                </li>
                <li>
                    <a href="https://github.com/Mahmoudreda66" style="color: #fff;"><i class="fab fa-github"></i></a>
                </li>
                <li>
                    <a href="mailto:mahmodreda219@gmail.com" style="color: #fff;"><i class="fas fa-envelope"></i></a>
                </li>
                <li>
                    <a href="tel:+201274385491" style="color: #fff;"><i class="fas fa-phone"></i></a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-image: url('https://images.pexels.com/photos/879109/pexels-photo-879109.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    color: #fff;
    padding: 20px 40px;
    position: relative;
    overflow: hidden;
    padding-bottom: 250px;

    nav {
        overflow: hidden;
        display: flex;
        align-items: center;

        .logo-area {
            font-size: 25px;
            font-weight: bold;
            float: left;
        }

        ul {
            float: left;
            list-style: none;
            margin-left: 80px;

            li {
                display: inline-block;
                margin-left: 15px;
                font-size: 17px;

                &.active {
                    color: #fff;
                    font-weight: bold;
                }
            }
        }
    }

    h1 {
        font-size: 40px;
        margin: 20px 0px;

        span {
            animation: h1Fade 1.4s infinite linear alternate;
        }
    }

    @keyframes h1Fade {
        from {
            opacity: .6;
        }

        to {
            opacity: 1;
        }
    }

    button.main {
        padding: 12px 30px;
        outline: none;
        border: 2px solid #ff392aac;
        background-color: #0000;
        color: #fff;
        border-radius: 3px;
    }

    .scroll-container {
        padding: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        width: 100%;
        bottom: 0px;
        right: 0px;
        left: 0px;

        .parent {
            border-radius: 30px;
            height: 70px;
            width: 35px;
            border: 3px solid #fff;
            display: flex;
            justify-content: center;
            padding: 10px 0px;
            cursor: pointer;

            span {
                width: 10px;
                height: 10px;
                background-color: #fff;
                border-radius: 50%;
                animation: mouseMove 1s infinite linear;
            }

            @keyframes mouseMove {
                from {
                    margin-top: 0px;
                }

                to {
                    margin-top: 30px;
                }
            }
        }
    }

    .icons {
        position: absolute;
        right: 40px;
        bottom: 10px;

        ul {
            list-style: none;

            li {
                margin-bottom: 20px;
                font-size: 20px;
            }
        }
    }
}
</style>

<script>
export default {
    methods: {
        scrollDown() {
            window.scrollTo(0, getComputedStyle(document.querySelector('header')).height.split('px')[0]);
        }
    },
    mounted() {
        document.querySelector('header').style.minHeight = window.innerHeight + 'px';
    }
}    
</script>