<template>
  <div>
    <Demo1/>
    <Icon name="arrow" class="icon"></Icon>
  </div>
</template>

<script>
import Demo1 from './components/Demo1.vue'

export default {
  name: 'App',
  components: {
    Demo1
  }
}
</script>

<style>
.icon{
  width: 50px;
  height: 50px;
}
</style>
