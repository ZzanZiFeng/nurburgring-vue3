<template>
  <div
    class="modal text"
    :class="[show && type == 'text' ? 'show' : '']"
    @click="$emit('close')"
  >
    <div class="inner" @click="innerModal">
      <div
        class="modal-content skew-n"
        v-html="content"
        @click="$emit('close')"
      ></div>
      <div class="modal-close skew-n" @click="$emit('close')">
        <svg viewBox="0 0 30 30">
          <circle cx="15" cy="15" r="12" />
          <path d="M10 10L20 20M20 10L10 20" />
        </svg>
      </div>
    </div>
  </div>

  <div
    class="modal image"
    :class="[show && type == 'image' ? 'show' : '']"
    @click="$emit('close')"
  >
    <div class="inner" @click="innerModal">
      <div class="modal-content skew-n" v-html="content"></div>
      <div class="modal-close skew-n" @click="$emit('close')">
        <svg viewBox="0 0 30 30">
          <circle cx="15" cy="15" r="12" />
          <path d="M10 10L20 20M20 10L10 20" />
        </svg>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// Props
defineProps({
  show: Boolean,
  type: String,
  content: String,
});

// Emits
defineEmits(["close"]);

// Methods
function innerModal(e) {
  e.stopPropagation();
}
</script>
