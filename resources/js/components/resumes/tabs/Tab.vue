<template>
  <BTab title-link-class="p-2">
    <template #title>
      <div class="d-flex justify-content-center">
        <div>
          <i :class="icon"></i>
        </div>
        <div>
          {{ title }}
        </div>
      </div>
    </template>
    <slot></slot>
  </BTab>
</template>

<script>
import BTab from 'bootstrap-vue';
export default {
  name: 'Tab',

  props: {
    title: {
      type: String,
    },
    icon: {
      type: String,
    },
  },

  components: {
    BTab,
  },
};
</script>
