<template>
  <form @submit.prevent="handleSubmit">
    <input v-model="text" type="text" placeholder="Search Jokes..." >
    <input type="submit" value="Search Jokes" >
  </form>
</template>

<script>
export default {
  name: 'SearchJokes',
  data () {
    return {
      text: ''
    };
  },
  methods: {
    handleSubmit () {
      this.$emit('search-text', this.text);
      this.text = '';
    }
  }
};
</script>
