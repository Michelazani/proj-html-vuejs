<script >
import MenuList from './MenuList.vue';
export default{
    name: 'AppHeader',
    data() {
        return {
        // arrray contenenti oggetti che utilizzerò nell'header
        menuHeader: [
                {
                    id: 1,
                    link: 'Home'
                },
                {
                    id: 2,
                    link: 'Apple'
                },
                {
                    id: 3,
                    link: 'Microsoft'
                },
                {
                    id: 4,
                    link: 'Android'
                },
                {
                    id: 5,
                    link: 'Forums'
                },
                {
                    id: 6,
                    link: 'Contact us'
                },
                {
                    id: 7,
                    link: 'Join us'
                },
            ]
            }
    },
    components:{
        MenuList
    }
}
</script>

<template>
    <header>
        <!-- upper header con logo img e ul -->
        <section class="upper-header">
            <div class="container upper-header">
                <img src="../assets/img/logo.png" alt="Avada Forum logo">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <MenuList v-for="menu in menuHeader" :linkMenu="menu.link"/>
                    <i class="fa-solid fa-magnifying-glass" style="color: #ffffff;"></i>
                </ul>
            </div>
        </section>
        <!-- middle header con text + btn -->
        <section class="middle-header">
            <div class="container">
                <h1>Tech Forum!</h1>
                <p>Discuss all the latest technology news and trends</p>
                <button class="btn btn-primary">get avada now! <span><i class="fa-solid fa-chevron-right" style="color: #ffffff;"></i></span> </button>
            </div>
        </section>
        <!-- lower header con text centrato  -->
        <section class="lower-header">
            <div class="s-container ">
                <h6> avada forum is the place to be</h6>
                <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. dolor at, bibendum purus. Dones vehicula nec tortor ac finibus. </p>
            </div>
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
        div.container{
            @include flex(row,space-between,center);
            ul{
                @include flex(row,center,center);
    
                list-style-type: none;
                color: white;
            }
            img{
                padding: 1rem 0;
                width: 12rem;
            }
        i.fa-magnifying-glass{
            font-size: small;
        }
        }

    }
    
    section.middle-header{
        background-image: url(../assets/img/home_slider_bg.jpg);
        height: 700px;
        background-size: contain;
        div{
            padding-top: 15rem;
            padding-left: 2rem;
        }
        h1{
        font-size: 7rem;
        font-weight: bolder;
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

    section.lower-header{
        background-color: $light-grey;
        text-align: center;
        div p{
            color: $dark-grey;
            padding: 1rem 0 4rem 0;
        }
    }
}

</style>