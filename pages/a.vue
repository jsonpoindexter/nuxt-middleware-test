<template>
  <div class="container">
    <div>
      <h1 class="title">
        Page A
      </h1>
      <div class="links">
        <nuxt-link to="/b">Go to Page B</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  middleware() {
    console.error("[a] ANON MIDDLEWARE");
  },
  beforeCreate: function() {
    console.error("[a] beforeCreate");
  },
  created: function() {
    console.error("[a] created");
  },
  beforeMount: function() {
    console.error("[a] beforeMount");
  },
  mounted: function(){
    console.error("[a] mounted");
  },
};
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
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
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
