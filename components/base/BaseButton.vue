<template>
  <button :class="[isDefault, isColor]" :type="isType" @click="onClick">
    <slot />
  </button>
</template>

<script>
export default {
  props: {
    type: {
      type: String,
      default: 'button',
    },
    color: {
      type: String,
      default: 'default',
    },
  },
  computed: {
    isColor() {
      switch (this.color) {
        case 'primary':
          return 'text-white bg-primary hover:text-white hover:bg-green-700 hover:border-green-700 cursor-pointer border-2 border-solid border-primary'
          break
        case 'secondary':
          return 'text-primary bg-white hover:text-white hover:bg-primary cursor-pointer border-2 border-solid border-primary'
          break
        case 'outline':
          return 'bg-white border-transparent text-dark'
          break
        default:
          return 'bg-silver-tree border-solid  text-white border-silver-tree cursor-pointer'
      }
    },
    isDefault() {
      return 'flex items-center justify-center font-medium font-general-sans rounded-100px text-20px-24px transition duration-500 ease'
    },
    isType() {
      switch (this.type) {
        case 'submit':
          return 'submit'
          break
        case 'reset':
          return 'reset'
          break
        default:
          return 'button'
      }
    },
  },
  methods: {
    onClick() {
      this.$emit('click')
    },
  },
}
</script>
