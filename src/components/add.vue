<template>
  <div>
    {{ n }}
    <button @click="add">+1</button>
  </div>
</template>

<script >


export default {

  data: function () {
    return {
      n: 0
    }
  },
  methods: {
    add() {
      this.n += 1
    }
  },
  created() {
    console.log("生成了")
  },
  updated() {
    console.log("更新了")
    console.log(this.n)
  },
  destroyed() {

    console.log('消亡了')
  }
}
</script>

<style lang="scss" scoped>

</style>