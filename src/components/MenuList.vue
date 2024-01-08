<script >

export default{
    name: 'MenuElement',
    // definisco le props che vado ad utilizzare nel MenuList
    props: [
        'linkMenu'
    ]
}
</script>

<template>
    <!-- scrivo la props che ho riportato nel vfor con :(nome props) tra le grafe  -->
    <li>{{ linkMenu }}</li>
</template> 

<style lang="scss" scoped>
li{
    padding: 0 1rem;
    font-size: small;
}
</style>