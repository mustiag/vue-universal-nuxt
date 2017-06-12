<template>
  <header>
    <div class="header">
      <div class="logo">
        <img src="~assets/images/ufc-logo.png"/>
      </div>
      <div class="nav">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/champions">Champions</nuxt-link>
      </div>
    </div>   
  </header>
</template>

<style>
.header
{
  min-height: 100px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin-bottom: 20px;
}
.logo img{
  height:70px;
  width: auto;
}
.nuxt-link-active
{
  color: grey ;
}
.title
{
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
.subtitle
{
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.nav
{
  padding-top: 15px;
}
.nav a
{
  padding: 10px;
  text-decoration: none;
}
</style>
