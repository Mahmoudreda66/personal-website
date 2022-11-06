<template>
    <section id="downloadCV" class="py-3 mt-3">
        <div class="container bg-white rounded p-4">
            <div class="row">
                <div class="col-md-6 col-12 mb-4 mb-md-0">
                    <h1 class="main-theme" style="margin-bottom: 0px;">
                        <span class="text">Download CV</span>
                        <div>
                            <span class="p">
                                <span></span>
                            </span>
                        </div>
                    </h1><br>
                    <p>Download My CV Now!</p>
                    <a :href="filePath">
                        <button class="btn btn-primary">
                            <i class="fas fa-download"></i> Download Full CV
                        </button>
                    </a>
                </div>
                <div class="col-md-6 col-12">
                    <img src="../../public/assets/jpg/Mahmoud_Reda.jpg" alt="cv" class="img-thumbnail">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default{
    data(){
        return {
            filePath: location.origin + '/Mahmoud_Reda.pdf'
        }
    }
}
</script>