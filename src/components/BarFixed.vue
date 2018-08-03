<template>
    <div
        class="barfixed"
        :style="{ backgroundColor: bgColor, color: textColor }"
        >
        <slot></slot>
    </div>
</template>

<script>
export default {
  name: 'Barfixed',
  props: {
    bgColor: {
      type: String
    },
    textColor: {
      type: String
    }
  }
}
</script>

<style lang="sass" scoped>
    .barfixed
      left: 0
      top: 0
      padding-top: 10px
      padding-bottom: 10px
      position: fixed
      width: 100%
</style>
