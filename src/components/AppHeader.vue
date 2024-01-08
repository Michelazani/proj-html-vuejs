<script >

export default{
    name: 'AppHeader',
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <header>
        
        <!-- upper header con logo img e ul -->
        <section class="upper-header">
            <div class="container">
                <div>
                    <img src="../assets/img/logo.png" alt="Avada Forum logo">
                </div>
                <ul>
                    <!-- li con props -->
                </ul>
            </div>
        </section>

            <!-- middle header con text + btn -->
        <section class="middle-header">
            <div class="container">
                <h1>Tech Forum!</h1>
                <p>Discuss all the latest technology news and trends</p>
                <button class="btn btn-primary">get avada now! > </button>
            </div>
        </section>

        <!-- lower header con text centrato  -->
        <section class="lower-header">

        </section>
            
        </header>
</template> 

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;

header{
    section.upper-header{
        background-color: $bluette;
    }
    h1{
        font-size: 7rem;
        font-weight: bolder;
    }
    img{
        padding: 1rem;
        width: 13rem;;
    }
    section.middle-header{
        background-image: url(../assets/img/home_slider_bg.jpg);
        height: 700px;
        background-size: contain;
        div{
            padding-top: 15rem;
            padding-left: 2rem;
        }
        p{
            color: white;
            padding: 2rem 0;
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
        }
    }
}

</style>