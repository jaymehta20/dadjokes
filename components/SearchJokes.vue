<template>
  <form @submit.prevent="onSubmit">
    <input type="text" v-model="text" placeholder="Search Jokes..." />
    <input type="submit" value="Search Jokes" class="btn" />
  </form>
</template>

<script>
export default {
  name: "SearchJokes",
  data() {
    return {
      text: ""
    };
  },
  methods: {
    onSubmit() {
      this.$emit("search-text", this.text);
      this.text = "";
    }
  }
};
</script>

<style>
input {
  padding: 5px 10px;
  margin: 5px;
  border: none;
  border-radius: 4px;
}
.btn {
  background-color: #000033;
  color: #fff;
  border: none;
  border-radius: 4px;
}
</style>
