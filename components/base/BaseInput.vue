<template>
  <div>
    <slot />
    <label v-if="label" class="block font-bold mb-1 text-primary" :for="name">
      {{ label }}
    </label>
    <input
      :id="name"
      :value="value"
      :type="type"
      :name="name"
      :placeholder="placeholder"
      :required="required"
      :class="[
        'bg-white',
        'border-light',
        'border-default',
        'border-solid',
        'text-light',
        'placeholder-light',
        'focus:ring-primary',
        'focus:border-primary',
        'rounded-100px',
        'py-19px',
        'px-25px',
        'w-full',
        'focus:outline-none',
        'focus:ring-1',
        'transition duration-500 ease',
        error && 'border-danger',
        classInput,
      ]"
      @input="$emit('input', $event.target.value)"
    />
    <p v-if="error" class="text-danger mt-2">{{ error }}</p>
  </div>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: '',
    },
    name: {
      type: String,
      default: '',
    },
    value: {
      type: [String, Number],
      default: '',
    },
    type: {
      type: String,
      default: 'text',
    },
    placeholder: {
      type: String,
      default: '',
    },
    required: {
      type: Boolean,
      default: false,
    },
    error: {
      type: String,
      default: '',
    },
    classInput: {
      type: String,
      default: '',
    },
  },
}
</script>
