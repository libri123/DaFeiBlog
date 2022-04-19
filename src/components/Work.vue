<template>
    <div class="work-exp">
        <h1 class="work-title">Career Roadmap</h1>
        <div class="work-grid">
            <workGridItem
            v-for="work in works"
            :key="work.id"
            :work="work" />
        </div>
  </div>
</template>

<script>
import { works } from "../data";
import workGridItem from "./partial/workGridItem.vue";

export default {
    name: "Work",
    components: {
        workGridItem,
    },
    data() {
        return {
            works,
        };
    }
}
</script>

<style scoped>
    .work-exp {
        overflow: auto;
        border: 5px solid lightblue;
    }
    .work-exp .work-title {
        width:100%;
        text-align: center;
    }
    .work-grid {
        display: flex;
        flex-direction: row;
    }
</style>
