<template>
  <div class="hello">
    <h4>{{ msg }}</h4>

    <ul>
      <img
        src="https://images.unsplash.com/photo-1601416137737-1806bc02d7f8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60"
      />

      <img
        src="https://images.unsplash.com/photo-1581560550192-5635c4e033c7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60"
      />
      <img
        src="https://images.unsplash.com/photo-1586991359975-54500b7d8a86?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=600&q=60"
      />
      <img
        src="https://embed-fastly.wistia.com/deliveries/49bd387c40e2c5aada92abdf973bc46d.webp?image_crop_resized=960x540"
      />
      <img
        src="https://i.ytimg.com/vi/-bAlWBbRtEw/maxresdefault.jpg?v=5f9b128f"
      />
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
