<template>
  <form
    class="d-flex justify-space-between align-center"
    @submit.prevent="handleSubmit"
  >
    <v-text-field
      v-model="text"
      class="search"
      type="text"
      label="Search Jokes..."
      color="indigo darken-4"
    />
    <v-btn
      type="submit"
      rounded
      color="indigo darken-4"
      value="Search Jokes"
      dark
    >
      Search
    </v-btn>
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

<style lang="scss" scoped>
.search {
  width: 15rem;
  flex: none;
}
</style>
