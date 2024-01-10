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
                    link: 'Proin at ligula sagittis vestibulum nisisì vitae'
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
        <div class="container">
            <section class=" upper-footer d-flex ">
                <div class="tech-forum">
                    <h6>avada tech forum</h6>
                    <p>Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras ei nibh risus. Pellentesque non mi sit amet mi intermentum.</p>
                </div>
                <div class=" popular-topics">
                    <h6>popular topics</h6>
                    <ul>
                        <!-- ciclo le props per il totale degli oggetti -->
                        <FooterListMenu v-for="popularTopic in popularTopics" :linkFooter="popularTopic.link" class="border-bottom" />
                    </ul>
                </div>
                <div class="recent-topics">
                    <h6>recent topics</h6>
                    <ul>
                        <!-- ciclo le props per il totale degli oggetti -->
                        <FooterListMenu v-for="recentTopic in recentTopics" :linkFooter="recentTopic.link" class="border-bottom"/>
                    </ul>
                </div>
                <div class="latest-replies">
                    <h6>latest replies</h6>
                    <ul>
                        <!-- ciclo le props per il totale degli oggetti -->
                        <FooterListMenu v-for="latestReply in recentTopics" :linkFooter="latestReply.link" class="border-bottom"/>
                    </ul>
                </div>
            </section>
        </div>
        <div class="border"></div>
        <div class="container">
            <section class="container lower-footer">
                <div class=" copyright">
                    <p> &#169; Copyright 2012-2020 | Avada Theme by <span class="black">Theme Fusion</span> | All rights reserved | Powered by <span class="black">WordPress</span></p>
                </div>
                <div class="icons">
                    <i class="fa-brands fa-facebook-f" style="color: #ffffff;"></i>
                    <i class="fa-brands fa-twitter" style="color: #ffffff;"></i>
                    <i class="fa-brands fa-instagram" style="color: #ffffff;"></i>
                    <i class="fa-brands fa-youtube" style="color: #ffffff;"></i>
                    <i class="fa-solid fa-chevron-up" style="color: #ffffff;"></i>
                </div>
            </section>
        </div>
    </footer>
</template> 

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;
    footer{
        section.upper-footer{
            padding: 3rem 0;
            ul{
            @include flex(column,center,start);
            list-style-type: none;
            }
            }
            .border-bottom{
                padding: 0.7rem 0;
                width: 87%;
            }
            h6{
                color: $black;
                padding-bottom: 1rem;
                padding-top: 1rem;
            }
            p{
                color: $dark-grey;
                padding: 0.7rem 0;
                font-size: 0.8rem;
            }
            div.tech-forum{
                width: 18rem;
                padding-right: 1.2rem;
            }
        }
        
        section.lower-footer{
            @include flex(row,space-between,center);
            p{
                color: rgb(122, 122, 122);
            }
            div.copyright p{
                font-size: 0.6rem;
            }
            span.black{
                color: black;
            }
            i{
                font-size: 1rem;
                margin: 1rem 0.5rem; 
                border-radius: 50%;  
                padding: 0.8rem;
            }
            i.fa-facebook-f{
                    background-color: $facebook;
                }
            i.fa-twitter{
                background-color: $twitter;
            }
            i.fa-instagram{
                background-color: $instagram;
            }
            i.fa-youtube{
                background-color: $youtube;
            }
            i.fa-chevron-up{
                border-radius: 0;
                background-color: $dark-grey;
                font-size: 0.5rem;
                padding: 0.3rem 0.5rem;
                position: absolute;
                top: 303rem;
                right: 5rem;
            }
        }
        .border{
            border-bottom: 3px solid $light-grey;
            width: 100%;
    }
        
   
</style>