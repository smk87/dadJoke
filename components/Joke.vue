<template>
  <div class="joke">
    <p>
      {{ joke }}
    </p>
  </div>
</template>

<script>
export default {
  name: 'Joke',
  props: ['joke', 'id']
};
</script>

<style>
.joke {
  padding: 1rem;
  border: 1px dotted #ccc;
  margin: 1rem 0;
}
</style>
