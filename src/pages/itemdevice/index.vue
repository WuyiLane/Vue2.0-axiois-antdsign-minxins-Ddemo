<template>
  <div class="app-container">
    <div class="demo-wrap">
      <div class="wrap-container">
        <div class="wrap-flex-item-f">
          <div class="demo-body">
            一号楼
            <div
              v-for="(item, index) in list.data"
              :key="index"
              class="demo-item"
              :style="{ top: -55* index + 'px',zIndex: 1000 - index }"
            >
              <!-- <div
            class="demo-item-devices demo-item-device-1"
            v-for="(p, i) in item.pionts"
            :key="i"
            :style="{ top: p.top, left: p.left }"
            @click="tap333"
          > -->
              <a-tooltip
                v-for="(p, i) in item.pionts"
                :key="i"
                :style="{ top: p.top, left: p.left }"
                @click="tap333"
              >
                <template slot="title">
                  {{ p.text }}
                </template>
                <div class="demo-item-devices demo-item-device-1"></div>
                <!-- Tooltip will show when mouse enter. -->
              </a-tooltip>
              <!-- </div> -->
              <!-- <div class="demo-item-device" @click="tap333">
            <div class="demo-item-devices demo-item-device-1"></div>
            <div class="demo-item-devices demo-item-device-2"></div>
            <div class="demo-item-devices demo-item-device-3"></div>
          </div>
          <div class="demo-item-device-item" @click="tap666">
            <div class="demo-item-devices demo-item-device-1-item"></div>
            <div class="demo-item-devices demo-item-device-2-item"></div>
            <div class="demo-item-devices demo-item-device-3-item"></div>
          </div> -->
            </div>
          </div>
        </div>
        <div class="wrap-flex-item-t">
          <div class="demo-body">
            二层楼
            <div
              v-for="(item, index) in list.data"
              :key="index"
              class="demo-item"
              :style="{ top: -55 * index + 'px',zIndex: 1000 - index }"
            >
              <!-- <div
            class="demo-item-devices demo-item-device-1"
            v-for="(p, i) in item.pionts"
            :key="i"
            :style="{ top: p.top, left: p.left }"
            @click="tap333"
          > -->
              <a-tooltip
                v-for="(p, i) in item.pionts"
                :key="i"
                :style="{ top: p.top, left: p.left }"
                @click="tap333"
              >
                <template slot="title">
                  {{ p.text }}
                </template>
                <div class="demo-item-devices demo-item-device-1"></div>
                <!-- Tooltip will show when mouse enter. -->
              </a-tooltip>
              <!-- </div> -->
              <!-- <div class="demo-item-device" @click="tap333">
            <div class="demo-item-devices demo-item-device-1"></div>
            <div class="demo-item-devices demo-item-device-2"></div>
            <div class="demo-item-devices demo-item-device-3"></div>
          </div>
          <div class="demo-item-device-item" @click="tap666">
            <div class="demo-item-devices demo-item-device-1-item"></div>
            <div class="demo-item-devices demo-item-device-2-item"></div>
            <div class="demo-item-devices demo-item-device-3-item"></div>
          </div> -->
            </div>
          </div>
        </div>
        <div class="wrap-flex-item-m">
          <div class="demo-body">
            三号楼
            <div
              v-for="(item, index) in list.data"
              :key="index"
              :style="{ top: -55 * index + 'px',zIndex: 1000 - index}"
              class="demo-item"
            >
              <!-- <div
            class="demo-item-devices demo-item-device-1"
            v-for="(p, i) in item.pionts"
            :key="i"
            :style="{ top: p.top, left: p.left }"
            @click="tap333"
          > -->
              <!-- <img :src="item.imgsrc" alt=""               class="demo-item"> -->
              <a-tooltip
                v-for="(p, i) in item.pionts"
                :key="i"
                :style="{ top: p.top, left: p.left }"
                @click="tap333"
              >
                <template slot="title">
                  {{ p.text }}
                </template>
                <div class="demo-item-devices demo-item-device-1"></div>
                <!-- Tooltip will show when mouse enter. -->
              </a-tooltip>
              <!-- </div> -->
              <!-- <div class="demo-item-device" @click="tap333">
            <div class="demo-item-devices demo-item-device-1"></div>
            <div class="demo-item-devices demo-item-device-2"></div>
            <div class="demo-item-devices demo-item-device-3"></div>
          </div>
          <div class="demo-item-device-item" @click="tap666">
            <div class="demo-item-devices demo-item-device-1-item"></div>
            <div class="demo-item-devices demo-item-device-2-item"></div>
            <div class="demo-item-devices demo-item-device-3-item"></div>
          </div> -->
            </div>
          </div>
        </div>
      </div>
      <div class="demo-body">
        YICENGLOU
        <div
          v-for="(item, index) in list.data"
          :key="index"
          class="demo-item"
          :style="{ top: -55 * index + 'px',zIndex: 1000 - index}"
        >
          <!-- <div
            class="demo-item-devices demo-item-device-1"
            v-for="(p, i) in item.pionts"
            :key="i"
            :style="{ top: p.top, left: p.left }"
            @click="tap333"
          > -->
          <a-tooltip
            v-for="(p, i) in item.pionts"
            :key="i"
            :style="{ top: p.top, left: p.left }"
            @click="tap333"
          >
            <template slot="title">
              {{ p.text }}
            </template>
            <div class="demo-item-devices demo-item-device-1"></div>
            <!-- Tooltip will show when mouse enter. -->
          </a-tooltip>
          <!-- </div> -->
          <!-- <div class="demo-item-device" @click="tap333">
            <div class="demo-item-devices demo-item-device-1"></div>
            <div class="demo-item-devices demo-item-device-2"></div>
            <div class="demo-item-devices demo-item-device-3"></div>
          </div>
          <div class="demo-item-device-item" @click="tap666">
            <div class="demo-item-devices demo-item-device-1-item"></div>
            <div class="demo-item-devices demo-item-device-2-item"></div>
            <div class="demo-item-devices demo-item-device-3-item"></div>
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import img from "../../assets/img.png";
export default {
  data() {
    return {
      list: {
        data: [
          {
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          },
          {
            index: 2,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "70px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "60px",
                text: "887878787"
              }
            ]
          },
          {
            index: 3,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          },
          {
            index: 4,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          },
          {
            index: 5,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          },
          {
            index: 6,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          },
          {
            index: 7,
            imgsrc: img,
            pionts: [
              {
                top: "20px",
                left: "10px",
                text: "77777"
              },
              {
                top: "20px",
                left: "30px",
                text: "77777666"
              },
              {
                top: "20px",
                left: "56px",
                text: "887878787"
              }
            ]
          }
        ]
      },
      message: "我是A点坐标?"
    };
  },
  methods: {
    tap333() {
      console.log(444);
    },
    tap666() {
      console.log(6666);
    }
  }
};
</script>

<style lang="scss" scoped>
.demo-wrap {
  margin-top: 300px;
  // 布局
  .wrap-container {
    display: flex;
    width: 85%;
    background: #36a9cf;
    margin: 10px auto;
    .wrap-flex-item-f {
      flex: 1;
      background: red;
    }
    .wrap-flex-item-t {
      flex: 1;
      background: rebeccapurple;
    }
    .wrap-flex-item-m {
      flex: 1;
      background: green;
    }
  }
  .demo-body {
    width: 300px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    .demo-item {
      position: relative;
      width: 116px;
      height: 122px;
    //   z-index: 999!important;
      background-color: #36a9cf;
      box-shadow: 0 3px 10px #444;
      transform: rotateX(50deg) rotate(45deg);
      .demo-item-devices {
        position: absolute;
        width: 10px;
        height: 10px;
        background-color: #ffffff;
        border-radius: 100%;
      }
      .demo-item-device {
        width: 50px;
        height: 50px;
        .demo-item-device-1 {
          bottom: 0;
          left: 100px;
        }
        .demo-item-device-2 {
          bottom: 200px;
          right: 0;
        }
        .demo-item-device-3 {
          bottom: 200px;
          right: 0;
        }
      }
      .demo-item-device-item {
        .demo-item-device-1-item {
          position: absolute;
          bottom: 0;
          left: 137px;
        }
        .demo-item-device-2-item {
          position: absolute;
          bottom: 200px;
          right: 0;
        }
        .demo-item-device-3-item {
          position: absolute;
          bottom: 200px;
          right: 0;
        }
      }
    }
  }
}
</style>
