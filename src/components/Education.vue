<template>
    <div class="education">
        <h1 class="education-title">Education</h1>
        <div class="education-grid">
            <educationGridItem
            v-for="education in educations"
            :key="education.id"
            :education="education" />
        </div>
  </div>
</template>

<script>
import { educations } from "../data";
import educationGridItem from "./partial/educationGridItem.vue";

export default {
    name: "Education",
    components: {
        educationGridItem,
    },
    data() {
        return {
            educations,
        };
    }
}
</script>

<style scoped>
    .education {
        overflow: auto;
        border: 5px solid lightblue;
    }
    .education-title {
        width:100%;
        text-align: center;
    }
</style>
