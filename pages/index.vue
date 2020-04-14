<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Going headless with Nuxt!
      </h1>
      <h2 class="subtitle">
        How to connect Nuxt.js with Storyblok
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
  <!-- <section>
    <component
      v-if="story.content.component"
      :key="story.content._uid"
      :blok="story.content"
      :is="story.content.component" />
  </section> -->
</template>

<script>
export default {
  components: {
    Logo
  },
  // data () {
  //   return {
  //     story: { content: {} }
  //   }
  // },
  // mounted () {
  //   // // Use the input event for instant update of content
  //   // this.$storybridge.on('input', (event) => {
  //   //   if (event.story.id === this.story.id) {
  //   //     this.$storybridge.resolveRelations(['featured-articles.articles'], (event) => {
  //   //       // event.story.content has now the resolved relations
  //   //       this.story.content = event.story.content
  //   //     })
  //   //   }
  //   // })
  //   // Use the bridge to listen the events
  //   this.$storybridge.on(['published', 'change'], (event) => {
  //     // window.location.reload()
  //     this.$nuxt.$router.go({
  //       path: this.$nuxt.$router.currentRoute,
  //       force: true,
  //     })
  //   })
  // },
  // asyncData (context) {
  //   // // This what would we do in real project
  //   // const version = context.query._storyblok || context.isDev ? 'draft' : 'published'
  //   // const fullSlug = (context.route.path == '/' || context.route.path == '') ? 'home' : context.route.path

  //   // Load the JSON from the API - loadig the home content (index page)
  //   return context.app.$storyapi.get('cdn/stories/home', {
  //     version: 'draft',
  //     resolve_relations: 'featured-articles.articles'
  //   }).then((res) => {
  //     return res.data
  //   }).catch((res) => {
  //     if (!res.response) {
  //       console.error(res)
  //       context.error({ statusCode: 404, message: 'Failed to receive content form api' })
  //     } else {
  //       console.error(res.response.data)
  //       context.error({ statusCode: res.response.status, message: res.response.data })
  //     }
  //   })
  // }
}
</script>
