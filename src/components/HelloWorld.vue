<template>
  <div class="hello">
    <div>
      <input v-model='username1'>
      <User :username='username1'></User>
    </div>
    <h1>VS</h1>
    <div>
      <input v-model='username2'>
      <User :username='username2'></User>
    </div>
  </div>
</template>

<script>
import User from './User'

export default {
  components: { User },
  name: 'HelloWorld',
  data () {
    return {
      username1: '',
      username2: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
.hello {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
</style>
