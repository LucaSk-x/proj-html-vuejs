<template>
    <div>
        <div class="top-nav">
            <div class="container">
                <div class="head d-flex justify-content-between align-items-center py-3">
                    <div class="left-head">
                        <span class="text-secondary pe-2">English</span>
                        <i class="fa-solid fa-chevron-down text-secondary"></i>
                    </div>
                    <div class="right-head">
                        <ul class="list-unstyled d-flex align-items-center">
                            <li class="text-secondary px-2" v-for="(headLink, i) in headLink" :key="i">{{headLink}}</li>
                            <i class="fa-brands fa-facebook text-secondary ps-2"></i>
                            <i class="fa-brands fa-twitter text-secondary ps-2"></i>
                            <i class="fa-brands fa-instagram text-secondary ps-2"></i>
                            <i class="fa-brands fa-linkedin text-secondary ps-2"></i>
                            <i class="fa-brands fa-google-plus text-secondary ps-2"></i>
                            <i class="fa-brands fa-youtube text-secondary ps-2"></i>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom-nav">
            <div class="container">
                <div class="bottom-head d-flex align-items-center py-3">
                    <div class="logo pe-5">
                        <div class="logo-ms"><img src="../../public/img/MasterStudy.svg" alt=""></div>
                    </div>
                    <div class="search d-flex align-items-center flex-grow-1 px-3">
                        <div class="category pe-3">
                            <i class="fa-solid fa-bars text-secondary pe-2"></i>
                            <span class="text-uppercase text-secondary">category</span>
                        </div>
                        <div class="search-courses w-75 flex-grow-1">
                            <div class="input-group">
                                <input type="text" class="form-control" placeholder="Search courses" aria-label="Recipient's username" aria-describedby="button-addon2">
                                <button class="my-btn" type="button" id="button-addon2"><i class="fa-solid fa-magnifying-glass text-white p-2"></i></button>
                            </div>
                        </div>
                    </div>
                    <div class="upgrades d-flex align-items-center ps-5">
                        <div class="instructor pe-4">
                            <i class="fa-solid fa-bullhorn text-secondary pe-2"></i>
                            <span class=" text-secondary">Become an Instructor</span>
                        </div>
                            <div class="instructor">
                            <i class="fa-solid fa-suitcase text-secondary pe-2"></i>
                            <span class=" text-secondary">for Enterprice</span>
                        </div>
                    </div>
                    <div class="sign-up d-flex align-items-center ps-5">
                        <div class="login pe-4">
                            <i class="fa-solid fa-user text-secondary pe-2"></i>
                            <span class="text-secondary">Log in</span>
                        </div>
                        <div class="sing-up pe-4">
                            <button class="fucs-up-btn text-uppercase"><strong>Sing up</strong></button>
                        </div>
                        <div class="save">
                            <i class="fa-solid fa-bookmark text-secondary"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="category-nav">
            <ul class="list-unstyled d-flex justify-content-center">
                <li class="text-white p-4" v-for="(link, i) in categoryLink" :key="i"><i :class="`${link.icon}`"></i><span class="ps-2">{{link.name}}</span></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            headLink: ['Home', 'Pages', 'Cours Formats', 'Courses', 'Demos',],
            categoryLink: [
                {name:'Business',icon:'fa-solid fa-money-bill-trend-up'},
                {name:'Design',icon:'fa-solid fa-palette'},
                {name:'Development',icon:'fa-solid fa-gear'}, 
                {name:'Lifestyle',icon:'fa-solid fa-face-smile'},
                {name:'Office productivity',icon:'fa-solid fa-print'},
                ]
        }
    }
}
</script>

<style lang="scss">
    .top-nav {
        border-bottom: 1px solid #dde6eb;

        ol, ul, dl {
        margin-top: 0;
        margin-bottom: 0;
        }
    }

    .bottom-nav {
        .form-control{
            border-radius: 0;
        }
        .my-btn {
            background-color: #457992;
            border: transparent;
        }

        .fucs-up-btn {
            background-color: #ff4550;
            color: white;
            padding: 1.5rem;
            border: unset;
            border-radius: 32px;
            letter-spacing: 1px;
        }
    }
    .category-nav {
        background-color: #292f47;
    }
</style>