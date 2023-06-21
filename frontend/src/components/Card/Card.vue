

<template>
    <div>
        <div>Title</div>
        <div>
            <Toggle v-model="checked"/>
    <p style="text-align: center">Toggle: {{ checked }}</p>
  </div>
        <div>Subtitle</div>
    </div>


</template>

<script>
import Toggle from "../Toggle/Toggle.vue";

export default {
  data() {
    return {
        checked: true
    };
  },
  components: {
    Toggle
  }
};


</script>

<style scoped>

</style>