<template>
  <div class="note">{{ note }}</div>
</template>

<script>
export default {
  name: 'Note',
  data() {
    return {
      note: '',
    };
  },
  props: {
    keyCode: String,
  },
  watch: {
    keyCode() {
      this.handleGlobalKeyDown(this.$props.keyCode);
    },
  },
  methods: {
    handleGlobalKeyDown(code) {
      switch (code) {
        case 'Digit1': // Key: 1
          this.note = 'C';
          break;
        case 'Digit2': // Key: 2
          this.note = 'D';
          break;
        case 'Digit3': // Key: 3
          this.note = 'E';
          break;
        case 'Digit4': // Key: 4
          this.note = 'F';
          break;
        case 'Digit5': // Key: 5
          this.note = 'G';
          break;
        case 'Digit6': // Key: 6
          this.note = 'A';
          break;
        case 'Digit7': // Key: 7
          this.note = 'H';
          break;
        case 'Digit8': // Key: 8
          this.note = 'C';
          break;
        // case 57:
        //    this.note = 'A';
        //    break;
        default:
          this.note = '';
      }
    },
  },
};
</script>
<style scoped>
.note {
  font-size: 25.5vw;
}
</style>
