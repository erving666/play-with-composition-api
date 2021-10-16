<template>
  <div id="login">
    <h1>Login</h1>
  </div>
</template>

<script>
import { ref, computed } from "vue";
export default {
  setup() {
    const capacity = ref(3);
    const attending = ref(["erving", "bob", "alice"]);
    const spaceleft = computed(() => {
      return capacity.value - attending.value.length;
    });

    function increase() {
      capacity.value++;
    }

    return { capacity, increase, spaceleft, attending };
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
