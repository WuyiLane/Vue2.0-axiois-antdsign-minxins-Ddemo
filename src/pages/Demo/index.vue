<template>
  <div class="app-container">
    <div class="demo-wrap">
      <div class="demo-body">
        <div
          v-for="(item, index) in list.data"
          :key="index"
          class="demo-item"
          :style="{ Top: -55 * index + 'px' }"
        >
          <div class="demo-item-device" @click="tap333">
            <div class="demo-item-form demo-item-device-1"></div>
            <div class="demo-item-form demo-item-device-2"></div>
            <div class="demo-item-form demo-item-device-3"></div>
          </div>
          <div class="demo-item-device-item" @click="tap666">
            <div class="demo-item-form demo-item-device-1-item"></div>
            <div class="demo-item-form demo-item-device-2-item"></div>
            <div class="demo-item demo-item-device-3-item"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: {
        data: [{}, {}, {}, {}, {}, {}, {}]
      },
      message: "我是A点坐标?"
    };
  },
  methods: {
      tap333(){
          console.log(444)
      },
      tap666(){
          console.log(6666)
      }
  }
};
</script>

<style lang="scss" scoped>
.demo-wrap {
  margin-top: 300px;
  .demo-body {
    width: 300px;
    margin: 0 auto;

    .demo-item {
      position: relative;
      width: 116px;
      height: 122px;
      background-color: #36a9cf;
      box-shadow: 0 3px 10px #444;
      transform: rotateX(50deg) rotate(45deg);

      .demo-item-device {
        .demo-item-device-1 {
          position: absolute;
          bottom: 0;
          left: 100px;
          width: 10px;
          height: 10px;
          background-color: #ffffff;
          border-radius: 100%;
        }
        .demo-item-device-2 {
          position: absolute;
          bottom: 200px;
          right: 0;
          width: 10px;
          height: 10px;
          background-color: #ffffff;
          border-radius: 100%;
        }
      }
      .demo-item-device-item {
        .demo-item-device-1-item {
          position: absolute;
          bottom: 0;
          left: 137px;
          width: 10px;
          height: 10px;
          background-color: #ffffff;
          border-radius: 100%;
        }
        .demo-item-device-2-item {
          position: absolute;
          bottom: 200px;
          right: 0;
          width: 10px;
          height: 10px;
          background-color: #ffffff;
          border-radius: 100%;
        }
      }
    }
  }
}
</style>
