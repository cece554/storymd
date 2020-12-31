<template>
  <section id="nav">
    <b-navbar class="nav-wrap">
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <h1 class="title">The Matcha Dealer</h1>
        </b-navbar-item>
      </template>
      <template slot="end">
        <b-navbar-item href="#">Contact</b-navbar-item>
      </template>
    </b-navbar>
  </section>
</template>
<style lang="scss">
@import '~bulma/sass/utilities/_all';
$primary: $white;
$link: $primary;
$link-invert: $primary-invert;
$link-focus-border: $primary;
$background: $orange;
$family-primary: $family-monospace;
$family-monospace: 'Roboto Mono';
$white: #f4efe9;
$orange: #a74815;
$text: $family-primary;

#app {
  font-family: 'Roboto Mono', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $primary;
  background: #a74815;
}

#nav {
  border-bottom: 1px solid #f4efe9;
  padding: 10px;

  a {
    font-family: Adieu;
    font-weight: 300;
    color: #f4efe9;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
  .title {
    color: #f4efe9;
    font-weight: 400;
  }
}
.navbar {
  background: #a74815;
}
.navbar-end .navbar-item {
  font-family: 'Roboto Mono' !important;
  text-transform: uppercase;
}
</style>
