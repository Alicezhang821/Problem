<template>
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
</template>
<script>
export default{
  name: 'PostsExample',
  data () {
    return {
      posts: [
        {id: 1, title: 'Post 1', body: 'kasfjk'},
        {id: 2, title: 'Post 2', body: 'kasfjk'},
        {id: 3, title: 'Post 3', body: 'kasfjk'}
      ]

    }
  }
}
</script>
