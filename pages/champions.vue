<template>
  <div>
    <navbar/>
    <section>
      <div class="row">
        <div class="col-md-3"  v-for="champ in champs">
          <card :key="champ.id" :champ="champ"></card>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import navbar from '~components/Navbar.vue'
import Card from '~components/Card.vue'
import axios from 'axios'

export default {
  asyncData ({ params, error }) {
    return axios.get('https://api.myjson.com/bins/x7j89')
    .then((res) => {
      return { champs: res.data }
    })
    .catch((e) => {
      error({ statusCode: 404, message: 'Post not found' })
    })
  },
  components: {
    navbar,
    Card
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
