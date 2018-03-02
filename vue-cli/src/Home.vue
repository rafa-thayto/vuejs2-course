<template>
  <div>
    <h1>Server status {{status}}</h1>
    <hr>
    <button @click='changeStatus'>Change Status</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      status: 'Critical'
    }
  },
  methods: {
    changeStatus () {
      if (this.status === 'Normal') {
        this.status = 'Critical'
        return
      } 
      this.status = 'Normal'
    }
  }
}
</script>


<style>

</style>

