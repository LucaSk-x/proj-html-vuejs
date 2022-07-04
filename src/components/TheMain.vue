<template>
    <div>
        <div class="udemy-affilate">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="description">
                            <h2 class="text-white fw-bold">Udemy Affiliate Sales</h2>
                            <h5 class="text-white">Monetize your audience and attract new customers with Udemy!</h5>
                        </div>
                    </div>
                    <div class="col slide-afflilate">
<!--                         <img class="slide-afflilate position-absolute" src="../../public/img/slide-1.jpg" alt="">
 -->                 </div>
                </div>
            </div>
        </div><!-- udemy-affilate -->
        <div class="popular-development">
            <div class="container">
                <div class="popular-development-card py-5">
                    <h4 class="fw-bold">Popular Development course</h4>
                </div>
                <div class="row">
                    <div class="col-2" v-for="product in developmentCourses" :key="product.title"></div>
                </div>
            </div>
        </div><!-- popular-development -->
        <div class="limitless-learning"></div><!-- limitless-learning -->
        <div class="recent-course"></div><!-- recent-course -->
        <div class="newsletter"></div><!-- newsletter -->
        <div class="popular-course"></div><!-- popular-course -->
        <div class="become-instructor"></div><!-- become-instructor -->
        <div class="investing-future"></div><!-- investing-future" -->
    </div>
</template>

<script>
export default {
    data() {
        return {
            developmentCourses: [
                {
                    img: "../../public/img/895786_7b4b_2-272x161.jpg",
                    type: "Development >",
                    title: "The complete iOS 10 & Swift 3 Developer course",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "../../public/img/246154_d8b0_3-272x161.jpg",
                    type: "Development >",
                    title: "Web design for beginners: Real word coding in HTML & CSS",
                    rating: "4",
                    discountPrice: "$129.99",
                    price: "$65",
                },
                {
                    img: "../../public/img/752950_b773-272x161.jpg",
                    type: "Development >",
                    title: "GitHub Ultimate: Master Git and GitHub - Beginnig to Expert",
                    rating: "4",
                    discountPrice: "$99.99",
                    price: "50",
                },
                {
                    img: "../../public/img/1253188_58f7_2-272x161.jpg",
                    type: "Development >",
                    title: "The complte iOS 11 & Swift Developer course - Build 20 Apps",
                    rating: "4",
                    discountPrice: "$199.99",
                    price: "$100",
                },
                {
                    img: "../../public/img/919872_ed54_6-272x161.jpg",
                    type: "Development >",
                    title: "Android Java Masterclass - Become an app Developer",
                    rating: "4",
                    discountPrice: "$99.99",
                    price: "$50",
                },
                {
                    img: "../../public/img/",
                    type: "Development >",
                    title: "Xamarin Forms: Build Native Cross-platform Apps with c#",
                    rating: "4",
                    discountPrice: "$189.99",
                    price: "$65",
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    .udemy-affilate {
        background-color: #ff4550;
        
        .description {
            padding: 7rem 1rem 7rem 7rem;
        }
        .slide-afflilate {
/*             right: 0;
            top: 0;
            bottom: 0;
            height: 100%;
            width: 50%; */
            background-image: url(../../public/img/slide-1.jpg);
            background-position: center;
            background-size: cover;
        }
    }
</style>