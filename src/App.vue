<template>
  <div id="app">
    <div id="flex-container">
      <div id="converter">
      <img src="https://shop.svggest.co/wp-content/uploads/2018/06/png-logo-curve-300x132.png">
      <h3>Packing Slip Converter</h3>
      <div>
      <!-- Styled -->
      <b-form-file v-model="file" :state="Boolean(file)" placeholder="Choose a file..."></b-form-file>
      <div class="mt-3">Selected file: {{file && file.name}}</div>
      <b-button id="generate">Convert & Download Packing Slip</b-button>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      file: null,
    }
  }
}
</script>

<style>
#flex-container {
  display: flex;
  justify-content: center;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#converter {
  background: #fefefe;
  height: 100%;
  width: 600px;
  margin-top: 200px;
  padding: 50px;
  border-radius: 5px;
}

h3 {
  margin-top: 15px!important;
  margin-bottom: 30px!important;
}

#generate {
  margin-top: 50px;
  background: #f2f2f2;
  color: #313131;
}
</style>
