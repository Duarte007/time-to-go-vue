<template>
  <a-button-group :size="size">
      <a-button class="btn back" type="primary">
        <a-icon type="left" />{{name}}
      </a-button>
    </a-button-group>
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
    name: String,
  }
}
</script>

<style>

</style>
