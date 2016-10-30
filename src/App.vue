<template>
  <div id="app">
    <left-panel></left-panel>
    <main-panel :curView="view"></main-panel>
  </div>
</template>

<script>
import leftPanel from './pages/left_panel'
import mainPanel from './pages/main_panel'

export default {
  name: 'app',
  data: function(){
    return {
      view: 'clinic'
    }
  },
  methods: {
    changeView: function(){
      alert('lll');
    }
  },
  events: {
    'change-view': function(){
      alert('jj')
    }
  },
  components: {
    leftPanel,mainPanel
  }
}
</script>

<style>
body,html{
  padding: 0;
  margin: 0;
  border: 0;
  height: 100%;
  width: 100%;
  font-size: 14px;
}
ul,li{
  margin: 0;
  padding: 0;
  border: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
