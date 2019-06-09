<template>
  <div>

    <header>
        TimeToGo - {{employee}}
    </header>

    <Trainee v-if="trainee"/>
    <Hired v-else/>

    <div class="progress">
      <Progress/>
    </div>

    <PrimaryButton :name="actionAdd"/>
    <PrimaryButton :name="actionCalc"/>


    <footer>
        Developed by: Duarte
    </footer>
  </div>
</template>

<script>
import Trainee from './Trainee.vue';
import Hired from './Hired.vue';
import PrimaryButton from './components/PrimaryButton.vue';
import DefaultButton from './components/DefaultButton.vue';
import Progress from './components/Progress.vue';

export default {
  name: 'app',
  data(){
    return{
      trainee: false,
      employee: "CLT",
      actionCalc: "Calcular",
      actionAdd: "Adicionar Intervalo"
    }
  },
  components: {
    Hired,
    Trainee,
    PrimaryButton,
    DefaultButton,
    Progress
  }
}
</script>

<style>
  @import './assets/css/styles.css';
</style>
