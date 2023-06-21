

<template>
    <div class="card">
        <div class="card-title">
            <h1>Title</h1>
            <span>
            <Toggle v-model:checked="checked"/>
            <span style="text-align: center">Toggle: {{ checked }}</span>
        </span>
        </div>
        
        <div class="card-subtitle">Subtitle</div>
    </div>


</template>

<script>
import Toggle from "../Toggle/Toggle.vue";

export default {
    data: () => ({
   checked: true,
  }),
//   data() {
//     console.log('1')
//     return {
//         checked: true
//     };
//   },
  components: {
    Toggle
  },
  watch: {
    checked() {
        this.setChecked();
    },
  },
  methods: {
    setChecked() {
      console.log('123');
    }
  }
};


</script>

<style scoped>

.card {
    border: 1px solid grey;
    border-radius: 5px;
}

</style>