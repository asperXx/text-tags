<template>
  <div class="text-tags-item">
    <div class="text-tags-item__title">{{ title }}</div>
    <div class="text-tags-item__tags">
      <div class="tags-item" v-for="(item, index) of tags" :key="index">
        <v-icon v-if="item.icon" class="mr-1">{{ item.icon }}</v-icon>
        <div class="tags-item__label">{{ item.label }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TextTagsItem",
  props: {
    title: String,
    tags: Object,
  },
};
</script>

<style lang="scss">
.text-tags-item {
  padding: 10px 5px;
  border-bottom: 1px solid rgb(174, 174, 174);
  color: rgb(58, 58, 58);
  &__title {
    font-size: 18px;
    font-weight: 600;
    color: rgb(29, 29, 29);
  }
  &__tags {
    display: flex;
    flex-wrap: wrap;
    height: 24px;
    overflow: hidden;
  }
  &:hover {
    color: rgb(248, 184, 66);
    .text-tags-item__title {
      color: rgb(248, 184, 66);
    }
    i.v-icon.v-icon {
      color: rgb(248, 184, 66);
    }
  }
}
.tags-item {
  display: flex;
  align-items: center;
  &:not(:first-child)::before {
    content: "";
    width: 2px;
    height: 2px;
    border: 3px solid;
    border-radius: 50%;
    margin-right: 4px;
  }
  &__label {
    font-size: 14px;
    margin-right: 10px;
  }
}
</style>
