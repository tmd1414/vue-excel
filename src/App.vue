<template>
  <div id="app">
    <v-excel v-model="data" :showRowHeader="true" :showColHeader="true" :showToolBar="true" ></v-excel>
  </div>
</template>

<script>
import VExcel from './components/Excel.vue'

export default {
  name: 'App',
  components: {
    VExcel
  },
  data () {
    return {

      data: {
        0:
            { 
              0:{
                text:"ss",
                canedit:true
                },
              1:{
                text:"bb",
                canedit:false
              }
            }
          ,
        rows:[
          {
            height:22
          },
          {
            width:200
          },
        ],
        cols:[
          {
             index:0,
             width:200
          }, 
          {
            index:1,
            width:200
          }
        ]
      }
    }
  },
  methods: {
    mousedown (evt) {
      console.log('::::mouse-down')
    },
    mousemove (evt) {
      console.log('::::mouse-move')
      return false
    },
    mouseup (evt) {
      console.log('::::mouse-up')
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0px;
  padding: 0;
}
</style>
