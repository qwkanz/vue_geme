<template>
  <div class="container">
 
    <Mondai class="board" title="問題" v-bind:message="mondai" />

    <Answer class="kaitou" answer="不正解" v-bind:message="kotae.A" />
    <Answer class="kaitou" answer="不正解" v-bind:message="kotae.B" />
    <Answer class="kaitou" answer="不正解" v-bind:message="kotae.C" />
    <Answer class="kaitou" answer="正解" v-bind:message="kotae.D" />
  </div>
</template>
      <style >
.board{
  width: 700px;
  text-align: center;
}
.kaitou{
  width: 500px;
  background-color:lightpink;
  margin-left: 100px;
  
  
}

</style>
<script>

import Mondai from "./components/Mondai.vue";
import Answer from "./components/Answer.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    // GoodBye,
    // Thankyou,
    Mondai,
    Answer,
  },
  data() {
    return {
      mondai: "奈良で一番高い山は？",
      kotae:{
        A:"A:若草山",
        B:"B:葛城山",
        C:"C:国見山",
        D:"D:八経ヶ岳"

      }
    };
  },
};
</script>