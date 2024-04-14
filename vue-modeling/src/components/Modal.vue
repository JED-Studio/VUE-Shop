<template>
  <div v-if="isOpen" class="modal">
    <div class="modal-content">
      <span class="close" @click="closeModal">X</span>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false
    }
  },
  methods: {
    openModal() {
      this.isOpen = true;
    },
    closeModal() {
      this.isOpen = false;
    }
  }
}
</script>

<style>
.modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal-content {
  background-color: white;
  padding: 20px;
  border-radius: 5px;
}

.close {
  position: absolute;
  top: 5px;
  right: 5px;
  cursor: pointer;
}
</style>