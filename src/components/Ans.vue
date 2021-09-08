<template>
  <div class="alert alert-primary" >
    <div ref="ans" v-on:click="doAction">{{ ans }}</div>
  </div>
</template>

<script>
export default {
  name: "Ans",
  props: {
    ans: String,
  },
  // data(){
    

  // },
  methods: {
    doAction() {
      if (this.ans === "C、眠くならないようにするため") {
        this.$refs.ans.innerHTML = "正解";
      }
    },
  },
};
</script>