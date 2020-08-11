<template>
  <div>
    <button @click="toggle">toggle</button>
    <hr>
    <Add v-if="visible===true"/>
  </div>
</template>

<script>

import Add from "@/components/add"
export default {
  components: {Add},
  data(){
    return  {
      visible:true
    }
  },
methods:{
    toggle(){

this.visible = !this.visible
      console.log(this.visible);
    }
}

};
</script>


<style lang="scss" scoped>

</style>