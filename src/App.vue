<template>
  <div>

    <header>
        TimeToGo - {{employee}}
    </header>

    <div class="content">

      <Radio/>

      <Trainee v-if="trainee"/>
      <Hired v-else/>

      <div class="progress">
        <Progress/>
      </div>

      <div id="button">
        <!-- <BackButton :name="actionBack"/> -->
        <PrimaryButton :name="actionAdd" :icon="'plus'"/>
        <PrimaryButton :name="actionCalc"/>
      </div>
      
    </div>



    <footer>
        Developed by: Duarte
    </footer>
  </div>
</template>

<script>
import Radio from './components/Radio.vue';
import Trainee from './Trainee.vue';
import Hired from './Hired.vue';
import PrimaryButton from './components/PrimaryButton.vue';
import BackButton from './components/BackButton.vue';
import Progress from './components/Progress.vue';

export default {
  name: 'app',
  data(){
    return{
      trainee: false,
      employee: "CLT",
      actionBack: "Voltar",
      actionCalc: "Calcular",
      actionAdd: "Adc. Intervalo"
    }
  },
  components: {
    Radio,
    Hired,
    Trainee,
    PrimaryButton,
    BackButton,
    Progress
  },
  methods:{
    consoleL: function(){
      console.log('entrei');
    }
  }
}
</script>

<style>
  @import './assets/css/styles.css';
</style>
