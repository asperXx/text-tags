<template>
  <div class="text-tags-container">
    <TextTagItem
      v-for="(item, index) of cards"
      :key="index"
      :title="item.title"
      :tags="item.tags"
    />
  </div>
</template>

<script>
import TextTagItem from "./TextTagsItem.vue";

export default {
  name: "TextTags",
  components: {
    TextTagItem,
  },
  props: {
    cards: Array,
  },
};
</script>

<style lang="scss">
.text-tags-container {
  width: 100%;
}
</style>
