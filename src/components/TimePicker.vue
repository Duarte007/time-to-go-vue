<template>
    <div class="content-fields">
        <label for="">{{label}}</label>
        <a-time-picker :defaultValue="moment('12:08', 'HH:mm')" format="HH:mm" />
    </div>
</template>
<script>
import moment from 'moment';
export default {
  methods: {
    moment,
  },
  props: {
    label: String
  }
}
</script>

<style>

</style>


