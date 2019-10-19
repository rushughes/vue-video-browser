<template>
  <div>
    <SearchBar @termChange="onTermChange" />
  </div>
</template>

<script>
import SearchBar from './components/SearchBar';
const API_KEY = process.env.API_KEY;

export default {
  name: 'App',
  components: {
    SearchBar
  },
  methods: {
    onTermChange(searchTerm) {
      console.log(searchTerm);
    }
  }
}
</script>

<style>
</style>
