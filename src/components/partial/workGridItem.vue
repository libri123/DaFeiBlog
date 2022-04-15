<template>
    <div class="work-item">
        <h2 class="step-number">{{ work.startYear }}</h2>
        <div class="step-arrow"></div>
        <h3 class="work-name">{{ work.title }}</h3>
        <ul class="work-description">
            <li v-for="item in work.description.split('.')" :key="item">
                {{ item }}
            </li>
            <br>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'workGridItem',
    props: ['work'],
}
</script>

<style scoped>
    .work-item {
        width: 80%;
    }
    .step-number {
        text-align: center;
    }

    .work-name {
        margin-left: 3%;
    }
    .work-description {
        margin-top: 3%;
    }
    .step-arrow {
        width: 280px;
        height: 40px;
        position: relative;
        background: #0d8ba1;
    }
    .step-arrow:after {
        content: "";
        position: absolute;
        border-left: 20px solid white;
        border-top: 20px solid transparent;
        border-bottom: 20px solid transparent;
        }
    .step-arrow:before {
        content: "";
        position: absolute;
        right: -20px;
        border-left: 20px solid #0d8ba1;
        border-top: 20px solid transparent;
        border-bottom: 20px solid transparent;
    }

    li {
        margin-top: 2%;
    }
</style>