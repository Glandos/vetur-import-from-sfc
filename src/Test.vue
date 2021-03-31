<template>
  <div>
    {{ foo }}
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

@Component
export default class Test extends Vue {
  foo = 1

  get innerFoo () {
    return this.foo
  }

  printFoo () {
    console.log(this.foo, "I'm foo from Test")
  }
}
</script>