<script >
import FooterListMenu from './FooterListMenu.vue';
export default{
    name: 'AppFooter',
    data() {
        return {
            popularTopics:[{
                    id: 1,
                    link: 'Nam a dolor volutpat massa auctor semper'
                },
                {
                    id: 2,
                    link: 'Sed euismod nunc urna fermentum arcu dapibus fringilla'
                },
                {
                    id: 3,
                    link: 'Cras lacinia tellus id mauris finibus lacus molestie'
                },
                {
                    id: 4,
                    link: 'Curabitur a scelerisque ligula'
                }
            ],
            recentTopics:[
                {
                    id: 1,
                    link: 'Cras lacinia tellus id mauris finibus lacus molestie'
                },
                {
                    id: 2,
                    link: 'Proin at ligula sagittis vesyibulum nisisì vitae'
                },
                {
                    id: 3,
                    link: 'Sed nec metus at est tincidunt elementum'
                },
                {
                    id: 4,
                    link: 'Nulla egestas nulla eu nulla suscipit molestie'
                }
            ],
            latestReplies:[
                {
                    id: 1,
                    link: 'Cras lacinia tellus id mauris finibus lacus molestie'
                },
                {
                    id: 2,
                    link: 'Cras lacinia tellus id mauris finibus lacus molestie'
                },
                {
                    id: 3,
                    link: 'Nulla egestas nulla eu nulla suscipit molestie'
                },
                {
                    id: 4,
                    link: 'Maurus ac nubh quis eros sagittis lacinia a et dui'
                }
            ]
        }
    },
    components:{
        FooterListMenu
    }
}
</script>

<template>
    <!-- 1.row ma ul in column con border-bottom
         2. border bottom 
         3. space between con icons
         4. position per ^ -->
    <footer>
        <section class="container upper-footer d-flex ">
            <div class=" popular-topics">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="popularTopic in popularTopics" :linkFooter="popularTopic.link" class="border-bottom" />
                </ul>
            </div>
            <div class="recent-topics">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="recentTopic in recentTopics" :linkFooter="recentTopic.link" class="border-bottom"/>
                </ul>
            </div>
            <div class="latest-replies">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="latestReply in recentTopics" :linkFooter="latestReply.link" class="border-bottom"/>
                </ul>
            </div>
        </section>
        <div class="border"></div>
        <section class="container lower-footer">
            <div class="copyright">
               <p> &#169; Copyright 2012-2020 | Avada Theme by <span class="black">Theme Fusion</span> | All rights reserved | Powered by <span class="black">WordPress</span></p>
            </div>
            <div class="icons">
                <i class="fa-brands fa-facebook" style="color: #3c5998;"></i>
                <i class="fa-brands fa-square-twitter" style="color: #54acee;"></i>
                <i class="fa-brands fa-square-instagram" style="color: #3f729b;"></i>
                <i class="fa-brands fa-square-youtube" style="color: #cd201f;"></i>
            </div>
        </section>
    </footer>
</template> 

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;
    footer{
        section.upper-footer{
            padding: 4rem 0;
            ul{
            @include flex(column,center,start);
            list-style-type: none;
            }
        }
        .border{
            border-bottom: 3px solid $light-grey;
            width: 100%;
        }
        .border-bottom{
            width: 80%;
        }
        section.lower-footer{
            @include flex(row,space-between,center);
            p{
                color: rgb(122, 122, 122);
            }
            div.copyright p{
                font-size: 0.8rem;
            }
            span.black{
                color: black;
            }
            i{
                font-size: 2rem;
                margin: 1rem 0.5rem;
            }
        }

    }
        
   
</style>