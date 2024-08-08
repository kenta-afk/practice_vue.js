<script setup>
defineProps({
    text: String,
});
const dataTest = "これはデータです！"
</script>



<template>
    <p>{{ text }}</p>
    <p>{{ dataTest }}</p>
</template>