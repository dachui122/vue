<template>
  <div class="person">
    <h2>当前求和为{{ sum }}</h2>
    <button @click="changeSum">点我sum加一</button>
  </div>
</template>
<script lang="ts" setup name="Person">
import { ref, watch } from 'vue'

//数据
let sum = ref(0)
//方法
function changeSum() {
  sum.value +=1
}
//监视

watch(sum,(_newvalue,_oldvalue)=>{
  console.log('sum变化了')
})
</script>





<style  scoped>
li{
  padding: 10px;
  margin: 0 5px;
}
.person{
    background-color: skyblue;
    box-shadow: 0 0 10px;
    border-radius: 10px;
    padding:10px;
}
button{
  padding: 10px;
  margin: 0 5px;
  
}
</style>