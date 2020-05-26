<template>
  <div>
    <label v-if="label">{{ label }}</label>
    <input :value="value" type="text" @input="updateValue" v-bind="$attrs" />
  </div>
</template>

<script>
import { formFieldMixin } from '../mixins/formFieldMixin'
export default {
  mixins: [formFieldMixin]
}
</script>