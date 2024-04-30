<template>
    <div class="app">
        <h1>你好啊</h1>
        <Person/>
</div>
</template>


<script lang="ts">
import Person from './components/Person.vue'

export default {
    name: 'App',
    components: {Person}//组件名
}
</script>
<style >
.app {
    background-color: #bf0808;
    box-shadow: 0 0 10px;
    border-radius:10px;
    padding:20px;
    margin:10px;
}
</style>