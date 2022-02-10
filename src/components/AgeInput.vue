<template>
  <div>
    <h2>Can you drive?</h2>
    <div class="d-flex">
      <input
        v-model="age"
        type="text"
        class="form-control"
        placeholder="Input your age"
      />
      <button class="btn btn-primary" @click="canTheyDrive">Enter</button>
    </div>
    <hr class="mb-4" />
    <div>
      <p>{{ result }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      result: "",
      age: "",
    };
  },
  methods: {
    canTheyDrive() {
      let inputAge = this.age;
      if (inputAge >= 18) {
        this.result = "Can drive";
      } else if (inputAge < 18 && inputAge >= 0) {
        this.result = "Cannot drive";
      } else this.result = "Error";
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
