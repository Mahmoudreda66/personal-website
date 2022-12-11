<template>
    <section id="workHistory" class="py-3 mt-3">
        <div class="container bg-white rounded p-4">
            <div class="row">
                <div class="col-12">
                    <h1 class="main-theme" style="margin-bottom: 0px;">
                        <span class="text">Work History</span>
                        <div>
                            <span class="p">
                                <span></span>
                            </span>
                        </div>
                    </h1><br>                    
                </div>
                <div class="col-12 mt-3">
                    <div>
                        <ul class="main-list">
                            <li class="mb-4 bg-light rounded p-3 main-li">
                                <h5>Fullstack (Laravel, Vue)</h5>
                                <p>Worked as fullstack web developer in diffrent freelancers & social media websites using php native or Laravel and Vue.js
                                </p>
                                <ul>
                                    <li>From: UNKNOWN</li>
                                    <li>To: 2022-10-1</li>
                                </ul>
                            </li>
                            <li class="bg-light rounded p-3 main-li">
                                <h5>Backend (Laravel)</h5>
                                <p>Worked as backend web developer in <a href="https://www.growtwopro.com/" target="_blank">GTP</a> (grow to pro) company</p>
                                <ul>
                                    <li>From: 2022-11-1</li>
                                    <li>To: STILL WORKING THERE</li>
                                </ul>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    ul.main-list{
        list-style: none;
        padding-left: 0px;

        h5{
            font-weight: 600;
        }

        li.main-li{
            &:hover{
                background-color: #f2f3f4 !important;
                transition: .4s;
            }
        }
    }
</style>

<script>
export default{
    // 
}
</script>