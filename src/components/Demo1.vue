<template>
  <div class="demo1">
    <svg width="100px" height="100px">
      <line x1="0" y1="50" x2="100" y2="50" stroke-width="8" stroke="currentColor"></line>
      <line x1="50" y1="0" x2="50" y2="100" stroke-width="8" stroke="#f00"></line>
    </svg>
    <svg width="100px" height="100px" viewBox="0 0 200 200">
      <line x1="0" y1="50" x2="100" y2="50" stroke-width="8" stroke="currentColor"></line>
      <line x1="50" y1="0" x2="50" y2="100" stroke-width="8" stroke="#f00"></line>
    </svg>

    <br>
    <svg width="300px" height="200px" viewBox="0 0 100 100" preserveAspectRatio="xMidYMid meet" style="border: 1px solid #000">
      <rect x="0" y="0" width="50" height="50" stroke-width="8" stroke="#f00" fill="none"></rect>
    </svg>

    <svg width="30px" height="30px" style="color: blue">
      <use href="#more"></use>
    </svg>

    <svg width="0" height="0">
      <defs>
        <symbol id="more" viewBox="0 0 100 100">
          <circle cx="20" cy="20" r="10" fill="currentColor"></circle>
          <circle cx="20" cy="50" r="10" fill="currentColor"></circle>
          <circle cx="20" cy="80" r="10" fill="currentColor"></circle>
          <line x1="40" y1="20" x2="100" y2="20" stroke-width="12" stroke="currentColor"></line>
          <line x1="40" y1="50" x2="90" y2="50" stroke-width="12" stroke="currentColor"></line>
          <line x1="40" y1="80" x2="100" y2="80" stroke-width="12" stroke="currentColor"></line>
        </symbol>

      </defs>
    </svg>

    <svg width="30px" height="30px" style="color: green">
      <use href="#play"></use>
    </svg>

    <svg width="30px" height="30px" style="color: deeppink">
      <use href="#arrow"></use>
    </svg>

    <svg width="0" height="0">
      <defs>
        <symbol id="play" viewBox="0 0 100 100">
          <polyline points="10 10 90 50 10 90" fill="currentColor"></polyline>
        </symbol>
        <symbol id="arrow" viewBox="0 0 100 100">
          <polyline points="10 10 90 50 10 90" fill="transparent" stroke-width="8" stroke="currentColor"></polyline>
        </symbol>
      </defs>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.demo1{
  color: #f00
}
</style>
