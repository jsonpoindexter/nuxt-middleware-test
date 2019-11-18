<template>
  <div class="container">
    <div>
      <h1 class="title">
        Page B
      </h1>
      <div class="links">
        <a href="https://www.google.com/search?aqs=chrome..69i57j69i60j69i61j69i60.508j0j4&sourceid=chrome&safe=active&q=foo&rlz=1c1gceb_enus851us851&ie=utf-8&oq=foo">Go To External</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  beforeCreate: function() {
    console.error("[b] beforeCreate");

  },
  created: function() {
    console.error("[b] created");
  },
  beforeMount: function() {
    console.error("[b] beforeMount");
  },
  mounted: function(){
    console.error("[b] mounted");
  },
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
