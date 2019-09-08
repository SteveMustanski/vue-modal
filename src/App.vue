<template>
  <div>
    <button class="btn" @click="openModal">Open Modal</button>
    <modal-direction :value="modalOpen"></modal-direction>
  </div>
</template>

<script>
import ModalDirection from "@/components/Modal";
export default {
  components: {
    ModalDirection
  },
  data() {
    return {
      modalOpen: false
    };
  },
  methods: {
    openModal() {
      this.modalOpen = !this.modalOpen;
    }
  }
};
</script>


<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #2c3e50; */

  margin-top: 60px;
}
</style>
