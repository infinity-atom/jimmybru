<script setup lang="ts">
    import Card from "./Card.vue";

    const { imgUrl } = defineProps({
        imgUrl: String
    });
</script>

<template>
    <card class="c">
        <div class="ia">
            <img :src="imgUrl" class="i">
        </div>
        <span class="l"><slot></slot></span>
    </card>
</template>

<style scoped>
    .c {
        display: flex;
        justify-content: space-between;
        align-items: center;

        flex-direction: column;
    }

    .i {
        border-radius: 10px;
        width: 200px;
    }

    .ia {
        display: flex;
        justify-content: center;
        align-items: center;
        flex: 1;
    }

    .l {
        font-size: 16pt;
        margin-top: 10px;
    }
</style>