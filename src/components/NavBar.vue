<template>
    <div>
        <nav class="navbar navbar-expand-lg fixed-top navbar-dark bg-dark navbar-custom">

            <div class="container-fluid">
                <!--LOGO IMAGE-->
                <!-- <a class="navbar-brand" href="#">
                    <img src="https://i.postimg.cc/HL6qqMXg/CSG099.png" width="100px" height="100px" alt="logo"
                        class="logo">
                </a> -->

                <div>
                    <!--COLLAPSE BUTTON-->
                    <button class="navbar-toggler m-0 p-0" type="button" data-bs-toggle="collapse"
                        data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                        aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                </div>

                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav mx-auto gap-5 text-black">

                        <!--MENU LIST-->
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i
                                    class="bi bi-house"></i>
                                <router-link to="/">    Home</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" id="product-section" href="#"><i
                                    class="bi bi-file-earmark-person"></i>
                                <router-link to="/about">   About</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i class="bi bi-folder2-open"></i>
                                <router-link to="/resume">  Resume</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i class="bi bi-wrench"></i>
                                <router-link to="/skills">  Skills</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i class="bi bi-controller"></i>
                                <router-link to="/projects">    Projects</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i class="bi bi-person-vcard"></i>
                                <router-link to="/testimonial"> Testimonial</router-link></a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#"><i class="bi bi-telephone"></i>
                                <router-link to="/contact"> Contact</router-link></a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {

}

</script>