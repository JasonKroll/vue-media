<template>
  <div id="app">
    <h1>Resize the window to see the effect:</h1>
    <media :query="{maxWidth: 800}">
      <div>
        <h2 style="color: orange">smaller than 800</h2>
        <h3>horay!</h3>
      </div>
    </media>
    <media :query="{minWidth: 800}">
      <div>
        <h2 style="color: green">bigger than 800</h2>
        <h3>oops!</h3>
      </div>
    </media>
  </div>
</template>

<script>
  import Media from '../src'

  export default {
    components: {
      Media
    }
  }
</script>
