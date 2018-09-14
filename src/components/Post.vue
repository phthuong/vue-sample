<script>
const Post = {
  template: '<div>Post: {{ $route.params.post_slug }}</div>',
  beforeRouteUpdate (to, from, next) {
    console.log(`Updating slug from ${from} to ${to}`)
    next() // make sure you always call next()
  }
}
export default Post
</script>
