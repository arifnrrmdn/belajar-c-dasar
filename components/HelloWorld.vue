<template>
  <div class="hello">
    <h1>MAN 2 Lebak</h1>
    <p>Learning Vue at Mandala Robotic Club</p>
    <input type="text" placeholder="Masukan nama kamu..." v-model="namamu">
    <p>{{ namamu }}</p>
    <button @click="greet(namamu)">Klik Disini</button>
  </div>
</template>


<script>
export default {
  name: 'HelloWorld',

  props: {
    msg: String
  },
  methods: {
    greet(namamu) {
      alert("Selamat Datang, " + namamu);
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  padding-top: 20px;
}

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
