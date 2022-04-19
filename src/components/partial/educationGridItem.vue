<template>
    <div class="education-item">
        <img v-bind:src="education.logourl" />
        <h3 class="education-name">{{ education.school }}</h3>
        <p class="education-period"> {{education.period }} <p>
        <p class="education-course">{{ education.course }}</p>
    </div>
</template>

<script>
export default {
    name: 'educationGridItem',
    props: ['education'],
}
</script>

<style scoped>
    .education-period {
        margin-right: 20%;
        float: right;
    }
    img {
        width: 12%;
        float: left;
    }
</style>