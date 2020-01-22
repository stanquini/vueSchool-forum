<template>
  <div>
    <h1>Welcome to the Forum</h1>
    <ThreadList />
  </div>
</template>

<script>
import sourceData from '@/data'
import ThreadList from '@/components/ThreadList'

export default {
  name: 'HelloWorld',
  components: {
    ThreadList
  },
  data () {
    return {
      threads: sourceData.threads,
      posts: sourceData.posts,
      users: sourceData.users
    }
  }
}
</script>
