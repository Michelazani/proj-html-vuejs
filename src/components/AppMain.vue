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
    7.div.container, calc/4
    8.ripeto 6
    9.bkg-img con text e btn 
    10. input+btn  -->
        <section>
        <div class="s-container">
            <h6>phasellus eget metus</h6>
            <h2>All the latest news</h2>
            <div class="line-bottom"></div>
        </div>
        <div class="container insert-img">
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
            <p>in quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
            <button type="button" class="btn btn-dark">read more ></button>
        </div>
        <div class="container insert-img">
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
        div.container.insert-img{
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
            background-image: url('../assets/img/featured_article_1_bg.jpg');
            height: 450px;
            background-size: 100%;
            text-align: start;
            padding: 0 5rem;
            h5{
                padding-top: 13rem;
                font-size: 0.9rem;
                text-transform: uppercase;
            }
            h3{
                padding: 1rem 0;
                font-weight: bold;
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
            }
        }
    }

</style>