<template>
  <div class="custom-button-with-props">
    <button
      class="button is-primary"
    >
      <span
        v-if="showIconBefore"
        class="custom-button-with-props__icon--before"
      >
        <i class="fas fa-arrow-right"></i>
      </span>
      <span v-if="buttonText.length">
        {{ buttonText }}
      </span>
      <span
        v-if="showIconAfter"
        class="custom-button-with-props__icon--before"
      >
        <i class="fas fa-arrow-right"></i>
      </span>
    </button>
    <!-- multiple, Icon, -->
  </div>
</template>

<script>
export default {
  name: 'CustomButtonWithProps',
  props: {
    buttonText: {
      type: String,
      default: '',
    },
    showIconBefore: {
      type: Boolean,
      default: false,
    },
    showIconAfter: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style>

</style>
