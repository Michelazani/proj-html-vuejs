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
        <section class="container upper-footer">
            <div class=" popular-topics">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="popularTopic in popularTopics" :linkFooter="popularTopic.link"/>
                </ul>
            </div>
            <div class="recent-topics">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="recentTopic in recentTopics" :linkFooter="recentTopic.link"/>
                </ul>
            </div>
            <div class="latest-replies">
                <ul>
                    <!-- ciclo le props per il totale degli oggetti -->
                    <FooterListMenu v-for="latestReply in recentTopics" :linkFooter="latestReply.link"/>
                </ul>
            </div>
        </section>
        <section class="lower-footer">

        </section>
    </footer>
</template> 

<style lang="scss" scoped>
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *;

   
</style>