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
    @use '../style/general.scss' as *;
    @use '../style/partials/mixins' as *;
    @use '../style/partials/variables' as *; 

li{
    padding: 0 1rem;
    font-size: small;
}
li:hover:after{
    content: "";
    display: block;
    width: 0;
	height: 0;
	border-left: 15px solid transparent;
	border-right: 15px solid transparent;
	border-top: 15px solid $bluette;
    position: absolute;
    top: 73px;
}

li:nth-child(7){
    text-transform: uppercase;
    font-weight: bold;
    background-color: $black;
    padding: 0.2rem 0.7rem;
    font-size: 0.7rem;
}
</style>