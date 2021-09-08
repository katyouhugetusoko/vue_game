<template>
  <div>
    <Que v-bind:que="mondai" />
    <Ans v-bind:ans="kotae.A" />
    <Ans v-bind:ans="kotae.B" />
    <Ans v-bind:ans="kotae.C" />
    <Ans v-bind:ans="kotae.D" />
  </div>
</template>

<script>
import Que from "./components/Que.vue";
import Ans from "./components/Ans.vue";

export default {
  name: "App",
  components: {
    Que,
    Ans,
  },
  data() {
    return {
      mondai:"おぼうさんが木魚をたたく意味はなんでしょう？？",
      kotae:{
            A:"A、お経にリズムをつけるため",
            B:"B、亡くなった人が天国にいけるようにと祈るため",
            C:"C、眠くならないようにするため",
            D:"D、悪い霊を寄せ付けないため",
      }
      
    }
  },
};


</script>