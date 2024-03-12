<template>
  <button type="button" @click="buttonClick">{{ label }}</button>
</template>

<script>
export default {
  name: "sample-button",
  props: {
    label: String,
  },

  methods: {
    buttonClick: (e) => {
      window.alert(`I'm a ${e.target.textContent}`);
    },
  },
};
</script>
