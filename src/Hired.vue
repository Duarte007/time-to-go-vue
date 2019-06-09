<template>
    <div class="content">

        <div id="coming">
            <TimePicker :label="labelComing"/>
        </div>

        <div id="intervals">
            <TimePicker :label="labelExitInterval"/>
            <TimePicker :label="labelComingInterval"/>
        </div>

        <div id="exit">
            <TimePicker :label="labelExit"/>
        </div>

    </div>
</template>

<script>
import TimePicker from './components/TimePicker.vue'

export default {
  name: 'app',
  data(){
      return{
          labelComing: 'Horário de chegada',
          labelExit: 'Horário de saída',
          labelExitInterval: 'Saída p/ Intervalo',
          labelComingInterval: 'Volta do Intervalo'
      }
  },
  components: {
    TimePicker
  }
}
</script>

<style>

</style>
