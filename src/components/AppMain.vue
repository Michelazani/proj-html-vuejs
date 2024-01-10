<script >

export default{
    name: 'AppMain',
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <main>
<!-- container per grandezza uguale . 
    1.text centrato  FATTO
    2. calc/3 + text
    3.background-img 100% con text e btn
    4.ripeto 2
    5.div diviso in 2 (60-40% ish)
    6. 100% black con text
    7.div.container, calc/4 con flex
    8.ripeto 6
    9.bkg-img con text e btn 
    10. input+btn  -->
    <section>
        <div class="s-container">
            <h6>phasellus eget metus</h6>
            <h2>All the latest news</h2>
            <div class="line-bottom"></div>
        </div>
        <div class="container images">
            <article>
                <img src="../assets/img/post_feat_img_25-320x202.jpg" alt="phone on a sofa">
                <h5><b>Morbi vitae dui euismod vulputate sollicitudin</b></h5>
                <p>October 11th, 2015 | <span>2 comments</span></p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
            <article>
                <img src="../assets/img/post_feat_img_24-320x202.jpg" alt="phone taking picture">
                <h5><b>Vivamus pellenteque, felis quis varius</b></h5>
                <p>October 11th, 2015 | Comments off </p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
            <article>
                <img src="../assets/img/post_feat_img_23-320x202.jpg" alt="watch img">
                <h5><b>Donec ornare pretium eget scelisque justo</b></h5>
                <p>October 11th, 2015 | Comments off </p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
        </div>
        <div class="container featured-article">
            <h5>featured article</h5>
            <h3>Cras malesuada et orci eget pharetra</h3>
            <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
            <button type="button" class="btn btn-dark">read more  <span><i class="fa-solid fa-chevron-right" style="color: #ffffff;"></i></span></button>
        </div>
        <div class="container images">
            <article>
                <img src="../assets/img/post_feat_img_22-320x202.jpg" alt="phone on a sofa">
                <h5><b>Fusce sollicitudin nunc sed placerat varius</b></h5>
                <p>October 11th, 2015 | Comments off </p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
            <article>
                <img src="../assets/img/post_feat_img_21-320x202.jpg" alt="phone taking picture">
                <h5><b>Donec facilis sodales leo sit amet laoreet</b></h5>
                <p>October 11th, 2015 | Comments off </p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
            <article>
                <img src="../assets/img/post_feat_img_20-320x202.jpg" alt="watch img">
                <h5><b>Proin eu purus sed aru aliquet curabir vens</b></h5>
                <p>October 11th, 2015 | Comments off </p>
                <p>Donec finibus sit amet orci eget ultricies. praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl</p>
            </article>
        </div>
        <div class="container d-flex">
            <div class="reviewed-product">
                <h5>reviewed product</h5>
                <h3>Mauris viverra atisan ipsum eget felis prims efficitur varius</h3>
                <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum.</p>
                <button type="button" class="btn btn-dark">read more ></button>
            </div>
            <div class="tutorials">
                <h4>Tutorials & Guides</h4>
                <div class="line-bottom"></div>
                <article class="d-flex single-box">
                    <img class="watch" src="../assets/img/post_feat_img_23-147x118.jpg" alt="watch img">
                    <div class="d-flex flex-column">
                        <h5><b>Donec ornare pretium eget scelisque justo</b></h5>
                        <p>October 11th, 2015 | Comments off </p>
                    </div>
                </article>
                <article class="d-flex single-box">
                    <img class="tablet" src="../assets/img/post_feat_img_22-147x118.jpg" alt="tablet img">
                    <div class="d-flex flex-column">
                        <h5><b>Fusce sollicitudin nunc sed placerat varius</b></h5>
                        <p>October 11th, 2015 | Comments off </p>
                    </div>
                </article>
                <article class="d-flex single-box">
                    <img class="phone" src="../assets/img/post_feat_img_20-147x118.jpg" alt="phone img">
                    <div class="d-flex flex-column">
                        <h5><b>Proin eu purus sed aru aliquet curabir vens</b></h5>
                        <p>October 11th, 2015 | Comments off </p>
                    </div>
                </article>
                
            </div>
        </div>
        <article class="black-line">
            <h5>read our blog <span><i class="fa-solid fa-arrow-right"></i></span> </h5>
        </article>
        <div class=" forum-section">
            <h6>phasellus eget metus</h6>
            <h2>Forum Sections</h2>
            <div class="line-bottom"></div>
            <div class=" container d-flex flex-row flex-wrap">
                <article class="sections news d-flex flex-column">
                    <i class="fa-solid fa-file-lines justify-content-center" style="color: #ffffff;"></i>
                    <h5><b>News & Community</b></h5>
                </article>
                <article class=" sections apple d-flex flex-column">
                    <i class="fa-brands fa-apple" style="color: #ffffff;"></i>
                    <h5><b>Apple Forum</b></h5>
                </article>
                <article class=" sections mictosoft d-flex flex-column">
                    <i class="fa-brands fa-windows" style="color: #ffffff;"></i>
                    <h5><b>Microsoft Forum</b></h5>
                </article>
                <article class=" sections android d-flex flex-column">
                    <i class="fa-brands fa-android" style="color: #ffffff;"></i>
                    <h5><b>Android Forum</b></h5>
                </article>
                <article class=" sections general d-flex flex-column">
                    <i class="fa-solid fa-mug-saucer" style="color: #ffffff;"></i>
                    <h5><b>General Discussion</b></h5>
                </article>
                <article class=" sections apps d-flex flex-column">
                    <i class="fa-solid fa-cubes" style="color: #ffffff;"></i>
                    <h5><b>Apps & Software</b></h5>
                </article>
                <article class=" sections gadgets d-flex flex-column">
                    <i class="fa-solid fa-laptop" style="color: #ffffff;"></i>
                    <h5><b>Gadget & Stuff</b></h5>
                </article>
                <article class=" sections tutorials d-flex flex-column">
                    <i class="fa-solid fa-wrench" style="color: #ffffff;"></i>
                    <h5><b>Tutorials & Guides</b></h5>
                </article>
            </div>
        </div>
        <article class="black-line">
            <h5>go to our forum <span><i class="fa-solid fa-arrow-right"></i></span> </h5>
        </article>
        <div class="join-community">
            <div class="s-container">
                <h2>Hey! Join to our Community</h2>
                <p>Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. Curabitur feugiat vulputate purus ipsums dolores ficilis uns etra.</p>
                <button class="btn "> sign up <span><i class="fa-solid fa-chevron-right" style="color: #ffffff;"></i></span> </button>
            </div>

        </div>
        <div class="newsletter"> 
            <div class="container">
                <p>Suscribe to our Newsletter</p>
                <input type="text" name="email" id="email" placeholder="Insert  your email*">
                <button type="button" class="btn btn-dark"> send</button>
            </div>
        </div>
    </section>

    </main>
</template> 

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;

    main{
        text-align: center;
        h2{
            font-weight: bold;
        }
        hr{
            width: 5rem;
            color: $light-orange;
        }
        div.line-bottom{
            padding-top: 1.5rem;
            width: 4rem;
            position: relative;
            left: 13rem;
            border-bottom: 0.1rem solid $light-orange;
        }
        div.container.images{
            width: calc(100% / 3);
            padding: 2rem 0.5rem 0 0.5rem;
            @include flex(row,center,stretch); 
            article{
                padding: 0 0.5rem;
            } 
            h5{
                font-size: 0.9rem;
                padding-top: 0.5rem;
                padding-bottom: 0.3rem;
            }
            h5,p{
                text-align: start;
                color: black;
                text-transform: inherit;
            }
            p{
                color:rgb(105, 105, 105) ;
                font-size: 0.8rem;
                padding-bottom: 0.5rem;

            }
            span{
                color: black;
            }
        }
        div.featured-article{
            margin-top: 2rem;
            margin-bottom: 2rem;
            background-image: url('../assets/img/featured_article_1_bg.jpg');
            height: 450px;
            background-size: 100%;
            text-align: start;
            padding: 0 5rem;
            h5{
                padding-top: 13rem;
            }
            h3{
                padding: 1rem 0;
                font-weight: bold;
            }
        }
        div.reviewed-product{
            margin-top: 2rem;
            margin-bottom: 2rem;
            width: 60%;
            height: 370px;
            background-image: url('../assets/img/featured_article_2_bg.jpg');
            background-size: 100%;
            background-position: center;
            text-align: start;
            h5,{
                padding: 5rem 0 1rem 3rem;
            }
            h3{
                padding: 0 3rem 1rem 3rem;
                font-weight: bold;
            }
            p{
                padding: 0 3rem;
            }
            button.btn{
                margin-left: 3rem;
            }
        }
        h5{
            font-size: 0.6rem;
            text-transform: uppercase;
        }
        p{
            font-size: 0.7rem;
        }
        h5,h3,p{
                color: white;
        }
        button.btn{
                border-radius: 0%;
                text-transform: uppercase;
                font-weight: bold;
                font-size: small;
                margin-top: 1rem;
                background-color: rgb(25, 25, 25);
        }
        
        div.tutorials{
            width: 40%;
            margin-top: 2rem;
            margin-bottom: 2rem;
            div.line-bottom{
                position: relative;
                left: 4rem;
            }
            h5,p{
                color: black;
                text-transform: inherit;
            }
            h4{
                font-weight: bold;
                text-align: start;
                padding-left: 4rem;
            }
            article.single-box{
                padding: 1.5rem 0 0 4rem;
                img{
                    width: 100px;
                }
                h5{
                    font-size: small;
                }
                h5,p{
                    padding: 0 1rem;
                    text-align: start;
                }
            }
        }
        article.black-line{
            background-color: rgb(25, 25, 25);
            height: 100px;
            @include flex(row,center,center);
            h5{
                font-weight: bold;
                font-size: small;
            }
        }
        div.forum-section{
            background-color: $light-grey;
            padding-bottom: 5rem;
            i{
                    background-color: $light-orange;
                    padding: 1rem;
                    font-size: 2rem;
                    border-radius: 50%;
                    width: 4rem;
                    margin: 0 auto;
                }
                h5{
                    margin: 1rem 0 2rem 0;
                }
            div.line-bottom{
                left: 45rem;
                margin-bottom: 2rem;
            }
            article.sections{
                width: calc((100% /4) - 2rem);
                margin: 1rem;
                padding: 1.5rem;
                display: flex;
                flex-wrap: wrap;
                background-color: white;
                border-top: 3px solid $bluette;
                h5,p{
                color: black;
                text-transform: inherit;
                font-size: smaller;
                }
            }
        }
        div.join-community{
            background-image: url(../assets/img/join_now_cta_bg.jpg);
            height: 450px;
            background-size: 100%;
            background-position: center;
            color: white;
            h2{
                font-size: 3rem;
                padding: 7rem 0 1.5rem 0;
            }
            button.btn{
            text-transform: uppercase;
            background-color: $bluette;
            border: transparent;
            border-radius: 0%;
            padding: 0.3rem;
            vertical-align: -moz-middle-with-baseline;
            font-weight: bold;
            font-size: smaller;
            padding: 0.5rem 2.5rem;
            color: white;
            }
            p{
                font-size: 0.8rem;
                padding-bottom: 1rem;
            }
        }
        div.newsletter{
            padding: 3rem 0;
            background-color: $light-grey;
            p{
                color: black;
                font-size: 1.5rem;
            }
            input{
                width: 400px;
                border: 0.5px solid lightgray;
                padding: 0.2rem 0.5rem;
                margin: 1rem 0 4rem 0;
            }
            button{
                text-transform: uppercase;
                margin: 0 1rem 0 2rem;
                padding: 0.3rem 4rem;
                vertical-align: baseline;
            }
        }
    }

</style>