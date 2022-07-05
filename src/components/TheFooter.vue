<template>
    <div class="foot">
        <div class="top">
            <div class="container">
                <div class="row justify-content-center pad">
                    <div class="col-3">
                        <div class="card-top p-3">
                            <h5 class="text-white text-uppercase pb-3">about</h5>
                            <p class="text-white">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nemo voluptatem ex magni quam, natus laudantium 
                                hic quod in vero obcaecati quibusdam libero fugiat voluptas aut sed aliquid, omnis qui pariatur.</p>
                        </div>
                    </div>
                    <div class="col-3">
                        <div class="card-top p-3">
                            <h5 class="text-white text-uppercase pb-3">Contact</h5>
                            <p class="text-white">USA, California 20, First Avenue, California</p>
                            <div class="text-white">Tel.: +1 212 456 789</div>
                            <div class="text-white pb-3">Fax: +1 252 45 45 20</div>
                            <p class="text-secondary">info@MasterStudy.com</p>
                        </div>
                    </div>
                    <div class="col-3">
                        <div class="card-top p-3">
                            <h5 class="text-white text-uppercase pb-3">social network</h5>
                            <div class="row gy-3">
                                <div class="col-3"><i class="fa-brands fa-facebook text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-instagram text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-linkedin text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-pinterest text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-twitter text-white"></i></div>
                                <div class="col-3"><i class="fa-solid fa-basketball text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-google-plus text-white"></i></div>
                                <div class="col-3"><i class="fa-brands fa-skype text-white"></i></div>
                            </div>
                        </div>
                    </div>
                    <div class="col-3">
                        <div class="card-top p-3">
                            <div class="top-udemy">
                                <img class="w-100" src="../../public/img/Top-udemy-courses-90-percent-off.jpg" alt="">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom p-3">
            <div class="container">
                <div class="bottom-card d-flex align-items-center">
                    <div class="foot-logo p-3">
                        <img class="w-50" src="../../public/img/footer-logo2x-50x56.png" alt="">
                    </div>
                    <div class="text-white ps-3">Copyrate © 2020. <span class="text-decoration-underline">Masterstudy.</span>Theme by <span class="text-decoration-underline">StylemixTheme</span></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
    .foot {
        background-color: #273044;
        .top {
            border-bottom: 1px solid rgba(202, 202, 202, 0.8);
            .pad {
                padding: 5rem 8rem 3rem 8rem;
                .card-top {
                    .fa-facebook {
                        background-color: #3b5998;
                    }
                    .fa-instagram {
                        background-color: #c32aa3;
                    }
                    .fa-linkedin {
                        background-color: #0077b5;
                    }
                    .fa-pinterest {
                        background-color: #bd081c;
                    }
                    .fa-twitter {
                        background-color: #1da1f2;
                    }
                    .fa-basketball {
                        background-color: #ea4c89;
                    }
                    .fa-google-plus {
                        background-color: #ea4c89;
                    }
                    .fa-skype {
                        background-color: #00aff0;
                    }
                    i {
                        font-size: 20px;
                        border-radius: 50%;
                        padding: .8rem  ;
                    }
                }
            }
        }
        .bottom-card {
            padding: 0 8rem;
        }
    }
</style>