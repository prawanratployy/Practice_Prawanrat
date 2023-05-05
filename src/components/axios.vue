<template>
  <div>
    <p v-for="manu in manufacturer" :key="manu.id">
      {{ manu.id }}- {{ manu.Title }}
      <input placeholder="="Id" v-model="id"/>
    </p>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      text: "test",
      manafacturer: [{ id: 1, Title: "test1" }],
    };
  },
  created() {
    this.get();
  },
  methods: {
    get() {
      //axios.get("https://localhost:7263/api/manufacturers")
      //.then((respone)
      //this.manafacturer = respone.data;
      //);
    },
  },
};
</script>