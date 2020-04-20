<template>
  <div class="alert-background">
    <div class="alert-wrapper">
      <div class="alert-header">
        <p>{{ title }}</p>
      </div>

      <div class="alert-body">
        <p>{{ msg }}</p>
      </div>
      <div class="alert-footer">
        <button @click="close">확인</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SimpleAlert",
  props: {
    msg: { default: "Alert Content", type: String },
    title: { default: "Alert Title", type: String },
  },
  methods: {
    close() {
      console.log("close");
      this.$destroy();
      this.$el.parentNode.removeChild(this.$el);
    },
  },
};
</script>

<style scoped>
.alert-background {
  top: 0;
  left: 0;
  position: absolute;
  background: rgba(0, 0, 0, 0.4);
  overflow: hidden;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
.alert-wrapper {
  width: 500px;
  height: 300px;
  background: white;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
}
.alert-header {
  border-bottom: 1px solid #eee;
  display: flex;
  justify-content: center;
  flex-basis: 40px;
}
.alert-body {
  flex: 1;
  overflow: auto;
}
.alert-footer {
  height: 60px;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}
.alert-body p {
  padding: 0 10px;
}

.alert-footer button {
  border: 1px solid #eee;
  height: 40px;
  width: 100px;
  background: white;
  box-shadow: none;
  cursor: pointer;
}

.alert-footer button:hover {
  background: rgba(255, 0, 0, 0.8);
  color: white;
}
</style>
