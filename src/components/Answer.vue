<template>
  <div class="alert alert-info">
    <div>
      <button class="container btn btn-info mt-2" v-on:click="doAction">
        <p class="text-success">{{ message }}</p>
      </button>
    </div>
  </div>
</template>



<script>
export default {
  name: "anser",
  props: {
    title: String,
    answer: String,
    message: String,
  },

  methods: {
    doAction() {
     if(this.answer=="正解"){
        window.alert("正解◎");
        }else{
          window.alert("不正解");
        }
      }
    },
 
}
</script>