<template>
    <p v-if="address != '' && town != ''"><i :class="icon"></i>&nbsp;{{title}}<br>{{address}}<br>{{town}}</p>
    <p v-else><i :class="icon"></i>&nbsp;{{title}}</p>
</template>

<script>
export default {
    name: 'FooterData',
    props: {
        icon: String,
        title: String,
        address: String,
        town: String
    }
}
</script>

<style>

</style>