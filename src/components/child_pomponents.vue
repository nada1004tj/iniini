<template>
  <div class="yellow lighten-3 pa-3">
    <h3>회원 정보 수정</h3>
    <p>수정내용</p>

    <button @click="childfunction">수정1</button>
  </div>
</template>
<script>
export default {
  data() {
      return{
        user:{}
      }
  },
  created() {
    this.user = "child user"
  },
  methods: {
    childfunction: function() {
       this.$emit("child",this.user)
    }
  }

}
</script>
