<template>
  <div>
    <h1>{{msg}}<br/>{{change}}<br/>{{shezhi}} 
   <span>oooo</span>
   <div class="title">mmmm</div>
    <br/></h1>
    <div>
    <button @click.self="add">clck</button>
    </div>
 
    <img src="../assets/logo.png" >

<mt-button
    type="primary"
    @click="sheetVisible = true">
    选择操作
  </mt-button>

  </div>
</template>

<script>
import { Button } from 'mint-ui';
  export default {
    name: 'moduleNmame',
    data() {
      return {
        msg: "msk"
      }
    },
    computed: {
      change() {
        return this.msg + "change"
      },
      shezhi:{
        set(){
          return this.msg+"set"
        },
        get(){
          return this.msg+"get"
        }
      }
    },
    methods: {
      add(){
        this.msg="hk";
      
      }
    }
  }
</script>

<style scoped >
:root{
  --cp:red;
  --wd:750px
}
  h1{
    width: var(--wd);
    height: 400px;
    border: 1px solid dashed;
    box-sizing: border-box;
    background: var(--cp);
    font-size: 50px;
    color:yellow;
   @nest & span{
    color: green;
  }
  }


</style>


