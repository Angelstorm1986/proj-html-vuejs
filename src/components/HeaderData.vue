<template>
    <li>
        <a href="#">
            <div class="choice" :class="{ active : active }">{{text}}</div>
        </a>
    </li>
</template>

<script>
export default {
    name: 'HeaderData',
    props: {
        text: String,
        active: Boolean
    }
}
</script>

<style>

</style>