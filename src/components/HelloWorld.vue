<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ prof }}</div>
  </div>
</template>

<script>
const title = function() {
  return `Mr. ${this.firstName} ${this.lastName}`;
};

const prof = function() {
  return `Prof. ${this.firstName} ${this.lastName}`;
};

export default {
  name: 'HelloWorld',
  data: () => ({
    firstName: 'Sam',
    lastName: 'Xiao',
  }),
  computed: {
    title,
    prof,
  },
};
</script>
