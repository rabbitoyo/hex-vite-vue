<script setup>
import { ref } from 'vue'

const num = ref(1)
console.log(num.value)
/*setInterval(() => {
num.value++
}, 500);*/

function clickMe() {
    num.value++
}
</script>

<template>
    <div>
        {{ num }}
        <button type="button" v-on:click="clickMe">點擊</button>
    </div>
</template>

<style scoped></style>
