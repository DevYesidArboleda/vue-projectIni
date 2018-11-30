<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
            <b-button size="lg" variant="success">Mi boton</b-button>
        </b-col>
        <b-col>
            <b-button :pressed="false">Mi boton</b-button>
        </b-col>
        <b-col>
            <b-button size="sm" variant="primary">Mi boton</b-button>
        </b-col>
      </b-row>

      <b-row>
        <b-row>Grid System</b-row>
      </b-row>
    </b-container>
    
    
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
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
