<template>
  <div class="layout">
    <!-- <header class="header"> -->
    <!--   <strong> -->
    <!--     <g-link to="/">{{ $static.metadata.siteName }}</g-link> -->
    <!--   </strong> -->
    <!--   <nav class="nav"> -->
    <!--     <g-link class="nav__link" to="/">Home</g-link> -->
    <!--     <g-link class="nav__link" to="/about/">About</g-link> -->
    <!--   </nav> -->
    <!-- </header> -->
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
}
</style>
