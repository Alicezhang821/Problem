<template>
  <div id="app">
  <table class="table table-striped mt4">
    <thead>
      <tr>
        <th scope="col">Id</th>
        <th scope="col">Title</th>
        <th scope="col">Body</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="post in posts" :key="post.id">
        <td>{{post.id}}</td>
        <td>{{post.title}}</td>
        <td>{{post.body}}</td>
      </tr>
    </tbody>
  </table>
  </div>
</template>

<script>
import PostsExample from './components/Posts'

export default {
  name: 'App',
  components: {
    PostsExample
  }
}
</script>

<style>
@import "../node_modules/bootstrap/dist/css/bootstrap.min.css";

#app {

}
</style>
