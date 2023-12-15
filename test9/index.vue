<template>
    <div>
        <Child>
            <template slot="add">
          <h1 slot="a1">a1</h1>
          <h1 slot="a2">a2</h1></template>
      <template scope="data">
      
        <ul>
            <li v-for="stu in data.student" :key="stu.index">{{ stu }}</li>
      </ul>
      </template>
        </Child>



    </div>
</template>
<script>
import Child from './child.vue'
export default {
    components: { Child },
    data() {
        return {
            
        }
    }
}
</script>
<style scoped></style>