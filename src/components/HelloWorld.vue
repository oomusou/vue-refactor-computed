<template>
  <div>
    <div>{{ title }}</div>
    <div>{{ prof }}</div>
  </div>
</template>

<script>
const fullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

const title = function() {
  return `Mr. ${this.fullName}`;
};

const prof = function() {
  return `Prof. ${this.fullName}`;
};

export default {
  name: 'HelloWorld',
  data: () => ({
    firstName: 'Sam',
    lastName: 'Xiao',
  }),
  computed: {
    fullName,
    title,
    prof,
  },
};
</script>
