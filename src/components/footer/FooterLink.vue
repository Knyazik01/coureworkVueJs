<template>
  <a v-if="linkUrl" :href="`${linkUrl}`">
    <img :src="getImgUrl(linkContent)" v-if="linkType === 'img'">
    <span v-else>{{linkContent}}</span>
    </a>
  <span v-else class="link">{{linkContent}}</span>
</template>

<script>
export default {
  name: "FooterLink",
  props: {
    linkUrl: String,
    linkContent: String,
    linkType: String,
  },
  methods: {
    getImgUrl(pic) {
      return require('@/assets/'+pic)
    }
  }
}
</script>

<style lang="scss" scoped>
.link {
  &:hover {
    color: #42b983;
  }
  color: red;
}
</style>