<script >

export default{
    name: 'MenuElement',
    // definisco le props che vado ad utilizzare nel MenuList
    props: [
        'linkFooter'
    ]
}
</script>

<template>
    <!-- scrivo la props che ho riportato nel vfor con :(nome props) tra le grafe  -->
    <li>
        <span><i class="fa-solid fa-chevron-right" style="color: #000000;"></i></span>
        {{ linkFooter }}
    </li>
</template> 

<style lang="scss" scoped>
span{
    font-size: 0.5rem;
    vertical-align: 1px;
}
li{
    font-size: 0.8rem;
}
</style>