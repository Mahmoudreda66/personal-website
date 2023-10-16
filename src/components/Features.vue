<template>
    <section id="features" class="py-3 mt-3">
        <div class="container bg-white rounded p-4">
            <h1 class="main-theme">
                <span class="text">Features</span>
                <div>
                    <span class="p">
                        <span></span>
                    </span>
                </div>
            </h1><br>
            <div class="row parent" style="margin-bottom: 20px;">
                <div class="col-md-4 col-sm-6 col-12 mb-3 mb-md-0 box">
                    <div class="content">
                        <img src="../../public/assets/png/coding.png">
                        <h4 class="mb-0">Hard Worker</h4>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-12 mb-3 mb-md-0 box">
                    <div class="content">
                        <img src="../../public/assets/png/Online_learning.png">
                        <h4 class="mb-0">Fast Learner</h4>
                    </div>
                </div>
                <div class="col-md-4 col-sm-6 col-12 mb-3 mb-md-0 box">
                    <div class="content">
                        <img src="../../public/assets/png/Php_document.png">
                        <h4 class="mb-0">Efficient Laravel Developer</h4>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
section#features {
    .parent {
        overflow: hidden;
        margin-top: 10px;

        img {
            width: 80px;
        }

        .box {
            h4 {
                margin: 20px 0px;
            }

            .content {
                padding: 15px;
                transition: .3s;

                &:hover {
                    background-color: #eee;
                    border-radius: 10px;
                    padding: 18px;
                }
            }
        }
    }
}
</style>