<template>
  <div>
    <navbar/>
    <section>
      <div class="jumbotron">
        <div class="">
          <h1 class="title">Welcome to the UFC Wiki</h1>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <h2 class="subtitle">About</h2>
          <p>
            The Ultimate Fighting Championship (UFC) is an American mixed martial arts-focused company,
            based in Las Vegas, Nevada, owned and operated by parent company William Morris Endeavor.
              It is the largest MMA promotion in the world and features the top-ranked fighters of the sport.
              Based in the United States, the UFC produces events worldwide that showcase ten weight divisions
                and abide by the Unified Rules of Mixed Martial Arts.
          </p>
        </div>
        <div class="col-md-6">
          <h2 class="subtitle">5 Fun Facts</h2>
          <ol>
            <li>There are rules - lots of them.</li>
            <li>
              The fighters' safety is top priority. If the ref feels that a fighter is not intelligently defending himself,
               they will not allow him to keep competing.
            </li>
            <li>
              MMA is considered to be safer than boxing because once a fighter is knocked out,
               they are not given a chance to get up and continue fighting.
            </li>
            <li>
              The reason the UFC uses an Octagon instead of a ring is for fighter safety.
            </li>
            <li>
              A championship fight goes for 5 rounds at 5 minutes each. 
            </li>
          </ol>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import navbar from '~components/Navbar.vue'

export default {
  components: {
    navbar
  }
}
</script>

<style>
.main
{
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
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
.links
{
  padding-top: 15px;
}
</style>
