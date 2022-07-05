<template>
    <div>
        <div class="udemy-affilate">    <!-- udemy-affilate -->
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="description">
                            <div class="text-white fw-bold display-5">Udemy Affiliate Sales</div>
                            <h4 class="text-white">Monetize your audience and attract new customers with Udemy!</h4>
                        </div>
                    </div>
                    <div class="col slide-afflilate"></div>
                </div>
            </div>
        </div>
        <div class="popular-development py-5">  <!-- popular-development -->
            <div class="container">
                <div class="popular-development-card pb-5">
                    <h4 class="fw-bold">Popular Development course</h4>
                </div>
                <div class="row">
                    <div class="col-2" v-for="product in developmentCourses" :key="product.title">
                        <TheCardProd 
                        :discountPrice="product.discountPrice"
                        :img="product.img"
                        :price="product.price"
                        :rating="product.rating"
                        :title="product.title"
                        :type="product.type"
                        >
                        </TheCardProd>
                    </div>
                </div>
            </div>
        </div>
        <div class="limitless-learning">    <!-- limitless-learning -->
                <div class="container">
                    <div class="row">
                        <div class="col-6">
                            <div class="description">
                                <div class="fw-bold display-5 pb-3">limitless learning, more possibilities</div>
                                <h4>Monetize your audience and attract new customers with Udemy!</h4>
                            </div>
                        </div>
                    <div class="col slide-afflilate"></div>
                </div>
            </div>
        </div>
        <div class="recent-course position-relative py-5">    <!-- recent-course -->
            <div class="container">
                <div class="recent-menu">
                    <h2 class="text-center fw-bold p-4">Recent course</h2>
                </div>
                <ul class="list-unstyled d-flex justify-content-center py-4">
                    <li class="pe-5 text-secondary" v-for="link in courseMenu" :key="link"> {{link}}</li>
                </ul>
                <div class="product-learning pe-5">
                    <div class="row gy-3">
                        <div class="col-2" v-for="product in recentCourse" :key="product.title">
                            <TheCardProd 
                                :discountPrice="product.discountPrice"
                                :img="product.img"
                                :price="product.price"
                                :rating="product.rating"
                                :title="product.title"
                                :type="product.type"
                                ></TheCardProd>
                        </div>
                    </div>
                </div>
                <button class="fucs-up-btn d-flex justify-content-center m-auto fw-bold text-uppercase my-5">show all</button>
                <div class="float-menu d-flex flex-column position-absolute p-3">
                    <i class="fa-solid fa-desktop text-secondary p-3"></i>
                    <i class="fa-solid fa-life-ring text-secondary p-3"></i>
                    <i class="fa-solid fa-wrench text-secondary p-3"></i>
                    <i class="fa-solid fa-cart-shopping text-secondary p-3"></i>
                    <i class="fa-solid fa-mobile-button text-secondary p-3"></i>
                </div>
            </div>
        </div>
        <div class="newsletter py-5">      <!-- newsletter -->
            <div class="container">
                <div class="row justify-content-center">
                    <div class="col-6">
                        <h4 class="fw-bold text-white">Subscribe our newsletter</h4>
                        <p class="text-white">There are many variation of passenger of Lorem ipsum available, 
                            but the majority have suffered alteration in some form, by injected humour, or randomize words</p>
                    </div>
                    <div class="col-4">
                        <h5 class="text-white text-uppercase">your e-mail address</h5>
                        <div class="input-group">
                            <input type="text" class="form-control" placeholder="Enter your E-mail" aria-label="Recipient's username" aria-describedby="button-addon2">
                            <button class="my-btn text-uppercase text-white p-2" type="button" id="button-addon2">subscribe</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="popular-course py-5">   <!-- popular-course -->
            <div class="container">
                <div class="recent-menu py-3">
                    <h2 class="text-center fw-bold pt-5">Recent course</h2>
                    <p class="text-center">Discover our most popular courses for self learning</p>
                </div>
                <div class="product-learning py-5">
                    <div class="row gy-3">
                        <div class="col-2" v-for="product in popularCourse" :key="product.title">
                            <TheCardProd 
                                :discountPrice="product.discountPrice"
                                :img="product.img"
                                :price="product.price"
                                :rating="product.rating"
                                :title="product.title"
                                :type="product.type"
                                ></TheCardProd>
                        </div>
                    </div>
                </div>
                <div class="pages d-flex justify-content-center m-auto py-4">
                    <div><i class="fa-solid fa-angle-left text-secondary p-3"></i></div>
                    <div><i class="fa-solid fa-angle-right text-secondary p-3"></i></div>
                </div>
            </div>
        </div>
        <div class="become-instructor">     <!-- become-instructor -->
            <div class="container">
                <div class="row p-5">
                    <div class="col-6">
                        <div class="instructor-card d-flex justify-content-center align-items-center p-5">
                            <div class="image-box"> <img class="h-100" src="../../public/img/image_box_1-221x231.png" alt=""></div>
                            <div class="description-instructor ps-5">
                                <h2 class="fw-bold pb-3">Become an Instructor</h2>
                                <p class="pb-3">Teach what you love. Masterstudy gives you the tools to create a course</p>
                                <button class="fucs-up-btn d-flex justify-content-center fw-bold text-uppercase">start teaching</button>
                            </div>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="instructor-card d-flex justify-content-center align-items-center p-5">
                            <div class="image-box"> <img class="h-100" src="../../public/img/image_box_2-234x231.png" alt=""></div>
                            <div class="description-instructor ps-5">
                                <h2 class="fw-bold pb-3">Access For Business</h2>
                                <p class="pb-3">Get unlimited access to 2.500 of top courses for your team</p>
                                <button class="fucs-up-btn d-flex justify-content-center fw-bold text-uppercase">Doing business</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="investing-future p-5">      <!-- investing-future" -->
            <div class="container">
                <div class="row">
                    <div class="col-7">
                        <div class="card-investing p-5">
                            <h2 class="fw-bold py-3">Investing for Your Future</h2>
                            <p class="pb-4">It is no exageration to say this Maststudy experience was transforming-both professionally and personally.
                                This Workshop will long remain a high point of my life. Thanks again.... I am feeling energized and aeger
                                to start teaching my class next week. I can't wait to use all ofmy new teaching tool. I will absolutely 
                                recommend this workshop to other educator! 
                            </p>
                            <div class="fw-bold">Linda Green</div>
                            <p class="text-secondary pb-3">Product Manager, Apple Inc.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import TheCardProd from './TheCardProd.vue'
export default {
    data() {
        return {
            developmentCourses: [
                {
                    img: "img/895786_7b4b_2-272x161.jpg",
                    type: "Development >",
                    title: "The complete iOS 10 & Swift 3 Developer course",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/246154_d8b0_3-272x161.jpg",
                    type: "Development >",
                    title: "Web design for beginners: Real word coding in HTML & CSS",
                    rating: "4",
                    discountPrice: "$129.99",
                    price: "$65",
                },
                {
                    img: "img/752950_b773-272x161.jpg",
                    type: "Development >",
                    title: "GitHub Ultimate: Master Git and GitHub - Beginnig to Expert",
                    rating: "4",
                    discountPrice: "$99.99",
                    price: "50",
                },
                {
                    img: "img/1253188_58f7_2-272x161.jpg",
                    type: "Development >",
                    title: "The complte iOS 11 & Swift Developer course - Build 20 Apps",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/919872_ed54_6-272x161.jpg",
                    type: "Development >",
                    title: "Android Java Masterclass - Become an app Developer",
                    rating: "4",
                    discountPrice: "$99.99",
                    price: "$50",
                },
                {
                    img: "img/951684_9c1a_2-272x161.jpg",
                    type: "Development >",
                    title: "Xamarin Forms: Build Native Cross-platform Apps with c#",
                    rating: "4",
                    discountPrice: "$189.99",
                    price: "$65",
                },
            ],/* "popular-development */
            courseMenu: ['All Categories','Business','Design','Development','IT & Software','Lifestyle','Marketing','Office Productivity',],/* recent-course */
            recentCourse: [
                {
                    img: "img/895786_7b4b_2-272x161.jpg",
                    type: "Development >",
                    title: "The complete iOS 10 & Swift 3 Developer course",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/246154_d8b0_3-272x161.jpg",
                    type: "Design >",
                    title: "CSS The Complete Guide 2020 (include Flexbox, Grid & Sass)",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/752950_b773-272x161.jpg",
                    type: "Development >",
                    title: "Web Design for Beginners: Real World Coding in HTML & CSS",
                    rating: "4",
                    discountPrice: "$129.99",
                    price: "65",
                },
                {
                    img: "img/1253188_58f7_2-272x161.jpg",
                    type: "design >",
                    title: "Digital Painting Light and Color: Amateur to Master",
                    rating: "4",
                    discountPrice: "$139.99",
                    price: "$70",
                },
                {
                    img: "img/919872_ed54_6-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Become an Arabic Calighaphic Artist from Scratch",
                    rating: "4",
                    discountPrice: "",
                    price: "$199.99",
                },
                {
                    img: "img/951684_9c1a_2-272x161.jpg",
                    type: "Google >",
                    title: "Google Searching Ninja",
                    rating: "4",
                    discountPrice: "$189.99",
                    price: "$45",
                },/*  */
                {
                    img: "img/949316_2a64_11-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Formation for Mastering Watercolor Painting",
                    rating: "4",
                    discountPrice: "$19.99",
                    price: "$10",
                },
                {
                    img: "img/366802_6fcc-272x161.jpg",
                    type: "Food & Beverage >",
                    title: "Get Wine-Smart",
                    rating: "4",
                    discountPrice: "$49.99",
                    price: "$25",
                },
                {
                    img: "img/381588_2e6d_4-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "The Colored pencil Drawing Course",
                    rating: "4",
                    discountPrice: "$34.99",
                    price: "18",
                },
                {
                    img: "img/1109398_4c13-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Paint realistic Watercolor and Botanicals - STUDIO BASIC",
                    rating: "4",
                    discountPrice: "$69.99",
                    price: "$35",
                },
                {
                    img: "img/1414956_d944_15-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Mastering Brushstrokes - Part 1",
                    rating: "4",
                    discountPrice: "$19.99",
                    price: "$10",
                },
                {
                    img: "img/1109398_4c13-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Paint Realistic Watercolor and Botanicals  - MAGNOLIAS",
                    rating: "4",
                    discountPrice: "$69.99",
                    price: "$35",
                },

            ],/* recent-course */
            popularCourse: [
                {
                    img: "img/895786_7b4b_2-272x161.jpg",
                    type: "Development >",
                    title: "The complete iOS 10 & Swift 3 Developer course",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/246154_d8b0_3-272x161.jpg",
                    type: "Design >",
                    title: "CSS The Complete Guide 2020 (include Flexbox, Grid & Sass)",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "img/752950_b773-272x161.jpg",
                    type: "Development >",
                    title: "Web design for beginners: Real word coding in HTML & CSS",
                    rating: "4",
                    discountPrice: "$99.99",
                    price: "50",
                },
                {
                    img: "img/1253188_58f7_2-272x161.jpg",
                    type: "Design >",
                    title: "Digital Painting Light and Color: Amateur to Master",
                    rating: "4",
                    discountPrice: "$139.99",
                    price: "$70",
                },
                {
                    img: "img/919872_ed54_6-272x161.jpg",
                    type: "Arts & Craft >",
                    title: "Become an Arabic Calighaphic Artist from Scratch",
                    rating: "4",
                    discountPrice: "",
                    price: "$199.99",
                },
                {
                    img: "img/951684_9c1a_2-272x161.jpg",
                    type: "Google >",
                    title: "Google search Ninja",
                    rating: "4",
                    discountPrice: "$189.99",
                    price: "$65",
                },
            ], /* popular course */
        };
    },
    components: { TheCardProd }
}
</script>

<style lang="scss">

    .udemy-affilate {
        background-color: #ff4550;
        background-image: url(../../public/img/slide-1.jpg);
        background-position: right;
        background-size: 50%;
        background-repeat: no-repeat;
        
        .description {
            padding: 9rem 1rem 9rem 7rem;
        }
    }
    .limitless-learning {
        background-image: url(../../public/img/bg.png);
        background-position: center;
        background-size: cover;

                .description {
                padding: 9rem 1rem 9rem 7rem;
        }
    }

    .recent-course {
        .fucs-up-btn {
            background-color: #ff4550;
            color: white;
            padding: 1.5rem;
            border: unset;
            border-radius: 32px;
            letter-spacing: 1px;
        }
        .float-menu {
            right: 0;
            bottom: 50px;
            box-shadow: -6px 0 10px rgb(219, 219, 219);
        }
    }

    .newsletter {
        background-color: #ff4550;

        .form-control {
            border-radius: 0;
        }
        .my-btn {
            background-color: #457992;
            border: transparent;
        }
    }
    .popular-course {
        background-color: #f0f4fa;

        .pages div {
            border: 1px solid rgb(228, 228, 228);
            background-color: #fff;
        }
    }

    .become-instructor {

        .instructor-card {
            border: 1px solid rgb(228, 228, 228); 
            .fucs-up-btn {
                background-color: #ff4550;
                color: white;
                padding: 1.5rem;
                border: unset;
                border-radius: 32px;
                letter-spacing: 1px;
            }
        }
    }
    .investing-future {
        background-image: url(../../public/img/testimonial-1-1917x640-1-1914x639.jpg);
        background-size: cover;
        background-position-y: center;

        .card-investing{
            background-color: #fff;
            margin-left: 15rem;
            p {
                letter-spacing: .8px;
                line-height: 18px;
            }
        }
    }

</style>