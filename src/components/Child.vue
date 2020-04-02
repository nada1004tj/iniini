<template>
  <div>
       <child_pomponents v-on:child="parents"></child_pomponents>
  </div>
</template>

<script>
import Vue from 'vue'
import child_pomponents from '@/components/child_pomponents'

export default {
  methods: {
    parents(message){
      alert(message);
    }
  },
  components: {
    child_pomponents
  }
}
</script>
