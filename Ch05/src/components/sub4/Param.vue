<template>
    <h4>Param</h4>
    <p>
        user : {{ user }}<br/>
        uid: {{ user.uid }}<br/>
        name: {{ user.name }}<br/>
        age: {{ user.age }}<br/>

    </p>
</template>
<script setup>
import { useRoute } from "vue-router";

// route 생성
const route = useRoute();

// params 데이터 수신
const user = route.params;
</script>
<style scoped></style>