<template>
    <div class="radio">
        <a-radio-group @change="setVisibility" defaultValue="a" :size="size">
        <a-radio-button value="a">CLT</a-radio-button>
        <a-radio-button value="b">Estágiario</a-radio-button>
        </a-radio-group>
    </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      size: 'large',
    }
  },
  props:{
    visibility: Boolean,
  },
  methods:{
    setVisibility: function(){
      this.trainee = !this.trainee;
    }
  }
}
</script>

<style>

</style>
