<template>
  <li>
    <div>Key:{{ this.$props.key }}</div>
    <input value="" maxlength="7" />
  </li>
</template>
<script>
export default {
  name: 'KeyAssignmentElement',
  data() {
    return {};
  },
  props: {
    key: String,
  },
};
