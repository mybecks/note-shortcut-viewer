<template>
  <div class="presets">
    <select>
      <option>C-Dur</option>
    </select>
    <ul>
      <li>
        <div>Key: 1</div>
        <input value="C" maxlength="3" />
      </li>
      <li>
        <div>Key: 2</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 3</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 4</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 5</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 6</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 7</div>
        <input value="" maxlength="3" />
      </li>
      <li>
        <div>Key: 8</div>
        <input value="" maxlength="3" />
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'Presets',
  data() {
    return {};
  },
  props: {
    keyCode: String,
  },
  watch: {
    keyCode() {
      this.handleGlobalKeyDown(this.$props.keyCode);
    },
  },
  methods: {},
};
</script>
<style scoped>
.presets {
  width: 100%;
  height: 10%;
  background-color: yellow;
  position: absolute;
  bottom: 0;
  left: 0;
}

.presets ul {
  list-style-type: none;
}

.presets li {
  display: block;
  width: 125px;
  border: 1px solid #000;
  float: left;
}

.presets input {
  width: 40px;
  text-align: center;
}
</style>
