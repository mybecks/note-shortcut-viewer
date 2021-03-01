<template>
  <div>
    <ul>
      <key-assignment-element key="1"><key-assignment-element>
      <key-assignment-element key="2"><key-assignment-element>
      <key-assignment-element key="3"><key-assignment-element>
      <key-assignment-element key="4"><key-assignment-element>
      <key-assignment-element key="5"><key-assignment-element>
      <key-assignment-element key="6"><key-assignment-element>
      <key-assignment-element key="7"><key-assignment-element>
      <key-assignment-element key="8"><key-assignment-element>
    </ul>
    <button>use</button>
  </div>
</template>
<script>
import KeyAssignmentElement from './components/KeyAssignmentElement.vue';

export default {
  name: 'KeyAssignment',
  components: {
    KeyAssignmentElement,
  },
  data() {
    return {};
  },
};
</script>
